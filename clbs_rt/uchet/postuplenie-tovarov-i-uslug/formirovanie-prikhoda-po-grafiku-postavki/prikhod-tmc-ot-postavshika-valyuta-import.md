---
title: Приход ТМЦ в валюте
description: Инструкция по созданию прихода от поставщика в валюте
published: true
date: 2022-09-14T05:18:36.123Z
tags: 
editor: markdown
dateCreated: 2022-08-31T08:59:04.024Z
---

# Приход ТМЦ в валюте

{% hint style="info" %}
Логистика > Управление документооборотом материальных и финансовых потоков > Документы > Реестр документов
{% endhint %}

Выбираем документ Приход ТМЦ от поставщика (валюта) (документ можно найти в строке поиска)

![](<../../../../.gitbook/assets/1 (125).png>)

## **Создание заголовка документа**

Далее нажимаем кнопку Добавить или клавишу на клавиатуре F7

![](<../../../../.gitbook/assets/2 (28).png>)

### Закладка Документ

* Склад и МОЛ
* Контрагент
* Договор
* Валюту и Курс валюты «Вводимый (ВВ)»
* Тип цены

{% hint style="info" %}
Курс РУБ к валюте рассчитываем в ручную исходя из курса валюты на день предоплаты и курса валюты на день прохождения Границы РФ
{% endhint %}

![](<../../../../.gitbook/assets/3 (27).png>)

{% hint style="info" %}
Если указан тип цены Плановая - такой документ в 1с выгрузится без цены!
{% endhint %}

### Закладка Документы

Указываем номер и дату входящего документа (ГТД)

{% hint style="info" %}
Документ не будет разнесен в картотеку,если не заполнена вкладка Документы
{% endhint %}

![](<../../../../.gitbook/assets/4 (32).png>)

## Создание строки документа

Нажимаем кнопку Добавить (F7). Или добавляем строки по Графику поставки (F2 - [Формирование прихода на основании графика поставки](../))

![](../../../../.gitbook/assets/5.png)

Заполняем поля документа:

### **Тип строки ТМЦ**

* код ТМЦ
* кол. док-т
* цену поставщика( в валюте), сумма рассчитывается автоматически (Сумму сверяем с коммерческим инвойсом)
* процент таможенной пошлины (указанный в ГТД.), таможенная пошлина может быть не на все ТМЦ

{% hint style="info" %}
После выполнения режима Рассчитать суммы оприходования по ГТД система автоматически создаст строку [Пошлина ](./#tip-stroki-poshlina)и рассчитаем сумму
{% endhint %}

* таможенную стоимость (указанная ГТД)

Нажимаем кнопку-Добавить.

![](<../../../../.gitbook/assets/6 (21).png>)

### **Тип строки Таможенный сбор**

* цена в руб. (указана в ГТД)
* отправитель указываем «Межрегиональное операционное УФК (ФТС России)»

Нажимаем кнопку-Добавить.

![](<../../../../.gitbook/assets/7 (44).png>)

### **Тип строки Пошлина**

{% hint style="info" %}
Создается только в том случае если необходимо распределить сумму на все строки прихода ТМЦ с одинаковым процентом
{% endhint %}

* цена и сумма с ТЗР ( берем из ГТД общую сумму по всем разделам)
* процент распределения
* признак распределения

Нажимаем кнопку-Добавить

![](https://firebasestorage.googleapis.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-MBaL4-sguLCzbQd3FRY%2Fuploads%2F2tWbJcP88BQ2hpUYARyx%2Ffile.jpeg?alt=media)

{% hint style="info" %}
После выполнения режима Рассчитать суммы оприходования по ГТД система автоматически в ТМЦ внесет процент и рассчитает сумму доп затрат пропорционально сумму ТМЦ
{% endhint %}

### **Тип строки Страхование**

* цена - берем из Страховки или акта выполненных услуг от Контрагента
* отправитель контрагент-страховщик
* договор
* дату документа .

![](<../../../../.gitbook/assets/9 (7).png>)

* № документа заполняем на вкладке «Дополнительно»

![](<../../../../.gitbook/assets/10 (10).png>)

Нажимаем кнопку «Добавить»

### **Тип строки ТЗР прочих контрагентов**

* цена берем из Акта выполненных работ от Контрагента
* отправитель контрагент- транспортная компания
* договор
* дату документа.

Номер документа заполняется на вкладке Дополнительно.

Нажимаем кнопку «Добавить»

![](<../../../../.gitbook/assets/11 (12).png>)

### Тип строки Прочие затраты

Аналогично заводим таможенное сопровождение и другие расходы, если возникнут

После заполнения всех Строк проверяем соответствие

* номенклатуры - количество
* суммы
* счета учета

![](<../../../../.gitbook/assets/12 (18).png>)

## Расчеты

### [Расчет по разделам ГТД](raschet-po-razdelam-gtd.md)

### Расчет суммы оприходования

Далее документ необходимо рассчитать. Устанавливаем курсор на строчные части документа (нижнее поле), нажимаем F2 => выбираем «Рассчитать суммы оприходования по ГТД»

![](<../../../../.gitbook/assets/13 (8).png>)

После расчета документа сравниваем итоговые значения в колонках «Сумма отпр.руб.» и «Сумма оприход. Руб.» - они должны быть равны (все затраты распределились правильно)

![](<../../../../.gitbook/assets/14 (22).png>)

Далее документ Передать вперед (в правом верхнем углу зеленая стрелка).

В поле экрана Реестр документов в колонке Рзн появился +. Документ разнесен в картотеку (проведен).

![](<../../../../.gitbook/assets/15 (1).png>)

> Отклонения в случае если спецификация с российским поставщиком заключена в валюте но приход необходимо оформить в рублях
>
> 1. Создаем заголовок валютного прихода и выбираем валюты спецификации
> 2. Формируем строки по графику поставок
> 3. Меняем валюту документа на рубли
> 4. Корректируем сумму и цену добавленных строк, указываем ставку НДС
>
> Расчет суммы оприходования по ГТД выполнять не нужно!