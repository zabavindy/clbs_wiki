---
title: Удаление DMS (план)
description: 
published: true
date: 2022-08-29T09:02:42.934Z
tags: 
editor: markdown
dateCreated: 2022-08-29T08:44:45.264Z
---

# Удаление DMS (план)

## **Как работает сейчас**

* Установка даты в таблице \_DMS\_DP

Что-то типа --Update \_DMS\_DP Set Stop =1--,DT\_DEL='20220301'

* Заполнение таблицы \_DMS\_L\_

В Планировщике F2. **Задача выполняется долго**&#x20;

![](<../../assets/image (1035).png>)

* Переключение DMS\_DP в режим работы

Update \_DMS\_DP Set Stop =0

* Запуск роботов DMS\_DEL\_\* (Количество выбираем от нагрузки)

**Для наглядности DMS\_DP**

![](<../../assets/0 (35)1.png>)

**ROWC** – по сколько строк захватывает каждый потом из DMS\_LOG

**STOP** – флаг регулировки включения роботов DMS\_DEL,

**CNT** – сколько строк нужно еще обработать, сейчас не используется

## **Как нужно сделать**

* Робот который запускается раз в месяц (Date\_Setter)и делает следующее:
  * Устанавливает дату в таблице \_DMS\_DP
  * Заполняет \_DMS\_L (Фактически нажимает F2)
  * Запускает 2-3 потока DMS\_DEL (медленно, но чтобы не нагружать БД)
* DMS\_DEL подкорректировать
  * чтобы актуальное количество поддерживать в DMS\_DP
  * Запускать только в “разрешенное время” ,например в 7.00 утра собственно как и сейчас, выключать перед ночными работать
  * Выключение при высоком CPU остается в силе
* DMS\_DEL\_CORRECTOR – робот – запуск раз в день, в “разрешенное” время, например в 7.00 утра, задачи:
  * А) проверить и актуализировать (при необходимости) количество в DMS\_DP
  * Б) Сбросить “мертвые”  сессии в DMS\_LOG (Если выключение происходило не штатным образом)
  * В) Если DMS\_DP количество больше 0, а роботы DMS\_DEL выключены, то включить этих роботов, и DMS\_DP set stop = 0

> А,Б – Это фактически автоматическая обработка сбойных ситуаций
{.is-info}
