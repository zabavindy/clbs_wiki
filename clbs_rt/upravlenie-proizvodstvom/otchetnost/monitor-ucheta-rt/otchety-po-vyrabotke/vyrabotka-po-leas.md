---
title: Выработка по LEAS
description: Отчет по расчету выработки по рабочим центрам LEA 
published: true
date: 2022-09-11T17:31:41.313Z
tags: 
editor: markdown
dateCreated: 2022-08-31T09:15:40.634Z
---

# Выработка по LEAS


>Управление производством → Управление производством и загрузкой мощностей (MRPII) → Журналы выработки и материальных потоков → Выработка


В появившемся фильтре указываем наименьший период, для более быстрой загрузки интерфейса, и нажимаем «ОК»

![](<../../../../assets/0 (83)1.png>)

После открытия интерфейса нажимаем F5 или нажимаем кнопку «Печать»

![](<../../../../assets/1 (71)1.png>)

В появившемся окне выбираем «Отчёт по выработке с переналадкой по LEAS» нажав 1 раз по нему и после нажимаем кнопку «Печать»

![](<../../../../assets/2 (60)1.png>)

Далее необходимо выбрать за какой период будет отобрана выработка

![](<../../../../assets/3 (47)1.png>)

После чего отчёт будет сформирован и выгружен пользователю

Для удобства просмотра отчёта закрепляем заголовки

![](<../../../../assets/4 (34)1.png>)

Также устанавливаем фильтр для сортировки по рабочим центрам

![](<../../../../assets/5 (27)1.png>)

Содержание отчёта

![](<../../../../assets/6 (23)1.png>)


>Желтым выделены строки, где осуществляется переход с одной модели на другую и только в них вычислено значение в поле «Переналадка»


Например, в двух нижних строчка на рабочем центре LEAS-2 осуществляется переход с модели 300x800 на 300x600 и в строке модели, на которую перешли, вычислено время переналадки

Строки отбираются по операции «Сварка» с количеством годных больше нуля

Колонки:

* Рабочий центр;
* Полное наименование оборудования;
* Характеристика оборудования;
* Техмаршрут заказа на производство;
* Смена;
* Дата смены;
* Начало выработки;
* Окончание выработки;
* Количество годных;
* Переналадка в минутах. 0 – если нет переналадки (выделены белым) или она не указана в системе;
* Количество работников по техмаршруту операции;
* Норма времени и расценки на 1 радиатор, значение в часах;
* Расчёт на нормативное количество работников, значение в часах


>Расчет: Норма времени и расценки на 1 радиатор \* кол-во годных


* Расчёт на одного рабочего, значение в часах


>Расчёт: Норма на нормативное количество работников / Количество работников по техмаршруту + Переналадка в минутах)

