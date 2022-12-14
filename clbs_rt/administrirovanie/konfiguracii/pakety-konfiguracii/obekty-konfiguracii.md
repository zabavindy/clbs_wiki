---
title: Объекты конфигураций
description: Инструкцию по объектам конфигураций
published: true
date: 2022-08-29T09:02:42.934Z
tags: 
editor: markdown
dateCreated: 2022-08-29T08:44:45.264Z
---

# Объекты конфигураций


* Объекты конфигурации
* [Добавление изменений в объект конфигураций](dobavlenie-v-obekt-konfiguracii.md)

## **Объекты конфигураций**

![](<../../assets/0 (88)1.png>)

* Пакеты для переноса на PROD
* Пакеты для разработки

## **RT (Пакеты для PROD)**

Формируется пакет с префиксом объекта и датой создания

## Разработка (по Фамильно)

Разработчик:

* Создаёт свою папку в пакете для разработок
* Добавляет в неё объекты конфигураций под необходимую разработку

![](<../../assets/1 (73)1.png>)

* После заполнения объекта конфигураций с разработками разработчик меняет предка на объект конфигураций, который будет сформирован следующим и не имеет заявки на установки из папки «RT (Пакеты для PROD)», и пишет в поле «Примечание» описание изменений, вносимых данным объектом конфигурации

![](<../../assets/2 (57)1.png>)

![](<../../assets/3 (49)1.png>)

Объекты конфигураций, которые не имеют заявки на установку отмечены знаком «-» в столбце «Статус заявки».

* После добавления в пакет для переноса на PROD необходимо встать на этот пакет (RT 20220318), нажать F2 и выбрать «Собрать элементы из дочерних объектов»

![](<../../assets/4 (33)1.png>)
