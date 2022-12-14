---
title: Тестирование КТД
description: Инструкция по тестированию качества конструкторско-технологических данных
published: true
date: 2022-09-11T17:31:41.313Z
tags: 
editor: markdown
dateCreated: 2022-08-31T09:15:40.634Z
---

# Тестирование КТД

## **Режим массового тестирования**

>Перейти в меню Управление производством → Техническая подготовка производства → Составы изделий → Тестирование комплектности технической документации


![](<../../assets/0 (96).png>)

Выбрать тип составов

![](<../../assets/1 (124).png>)

Далее проходит операция тестирования, может занять несколько минут.

Собственно, перед нами открывается окно с некорректными составами. Слева список тестов, справа обобщенные данные

## Список ошибок

### 1.Нормы

![](<../../assets/2 (4).png>)

Переключившись на нормы, вы увидите составы, которые не соответствуют условию **У Всех учетных операций есть норма времени и расценки и норма использования оборудования и они больше 0**. Встав на конкретную позицию, в нижней части экрана отобразиться некорректный маршрут, с возможностью перехода (F12).

![](<../../assets/3 (68).png>)

![](<../../assets/4 (27).png>)

### 2. Проверка норм отходов

![](<../../assets/5 (17).png>)

У Указанных ДСЕ в ссылочном технологическом процессе отсутсвует норма отхода (902), хотя в групповом тех.маршруте (O00000000000000) указана

### 3. Наличие ТП

![](<../../assets/6 (67).png>)

Вы увидите ДСЕ собственного производства (из строк спецификаций), которые не имеют технологического маршрута

### 4. Сверка признаков изготовления и раздела документации c KSM![](<../../assets/7 (10).png>)

Вам будут показаны ДСЕ где не совпадает значение полей ресурса (KSM) и строки спецификации

* Раздел Документации (KTKP)
* Признак Изготовления (KSP1)

Также в выборку попадают строки если KSM<>KSMO по указанным полям

### 5. Проверка наличия спецификаций или норм основного материала![](<../../assets/8 (50).png>)

>Анализируем только те, что с признаком собственное производство, покупные в анализ не попадают

* отсутствует спецификация технологическая (902)
* указанные ДСЕ не используются нигде в качестве нормы расходования основных материалов (901)
* указанные ДСЕ не являются исполнениями (Таблица TKSZ)

### 6. Проверка наличия спецификаций

&#x20;![](<../../assets/9 (31).png>)

>_Анализируем только те, что с признаком знаком разузловка, как покупные так и собственного производства, но не детали_

* отсутствует спецификация технологическая (902)
* указанные ДСЕ не используются нигде в качестве нормы расходования основных материалов (901)
* указанные ДСЕ не являются исполнениями (Таблица TKSZ)

### &#xD;**7.  Проверка признака выверено в спецификации**


Будет выведен список кодов ДСЕ, который связан с той спецификацией к которой нет признака вывереки

>Анализируем только те, что с признаком знаком разузловка, как покупные так и собственного производства, но не детали

![](<../../assets/image (454).png>)

Перейти к спецификациям можно по клавише F12, по пункту «Перейти к спецификации»

![](<../../assets/image (241).png>)

### **8.**&#xD;**Проверка признака выверено тех. маршрутов**

Будет выведен список **** кодов ДСЕ, который связан с тех. маршрутом, у которого отсутствует признак выверенности. Анализируем, групповые и единичные тех.маршруты

![](<../../assets/image (86).png>)

Перейти к тех. маршруту можно по клавише F12, по пункту «Перейти к тех. маршруту»

![](<../../assets/image (455).png>)

## Тестирование выбранного состава

Для тестирования одного состава достаточно на строке состава нажать f12 и выбрать “Тестирование комплектности техдокументации”. При это все тесты описанные ранее будут проделаны для одного выбранного состава

![](<../../assets/10 (9).png>)
