---
description: Инструкция по формированию спецификации
---

# Создание спецификации на закупку

## **Формирование спецификации по тендеру**

Спецификация формируется автоматически на основании выбранного победителя в тендере. Для этого тендер должен быть на стадии "Формирование спецификации" по внесенным предложениям должен быть выбран победитель

![](<../../.gitbook/assets/image (873).png>)

С заголовка документа вызываем метод "Формирование спецификации к договору" (F2 - Формирование спецификации к договору) библиотеки кода C# - SCENARIOS

![](<../../.gitbook/assets/image (196).png>)

Заполняем основные реквизиты спецификации

* Номер поставщика и дата
* Тип спецификации (Счет или спецификация)
* Договор (подставляется первый действующий). Если несколько действующих договоров необходимо выбрать руками (F10 из поля Договор)

![](<../../.gitbook/assets/image (845).png>)

После нажатия ОК сформируется спецификация

Остальные поля необходимо заполнить перейдя в спецификацию. Смотри инструкцию ниже

{% hint style="danger" %}
При формировании спецификации проверяется дата окончания срока действия договора. Если срок действия истек, то высветится ошибка "Срок действия договора истек!". Проверка внутри кода библиотеки SCENARIOS
{% endhint %}

{% hint style="info" %}
Если было несколько победителей сформируется спецификация на каждого победителя по своей номенклатуре
{% endhint %}

После создания номер спецификации будет виден в заголовке тендера. Двойным щелчком можно перейти в нее

![](<../../.gitbook/assets/image (188).png>)

## **Формирование спецификаций без плана закупа**

{% hint style="info" %}
На спецификацию сформированную руками нельзя будет сформировать график поставки. Т.е. система не увидит материалы в пути
{% endhint %}

Открыть Реестр документов - Выбрать тип процесса Спецификация на закупку

![](<../../.gitbook/assets/image (438).png>)

Создаем заголовок документ

Закладка **Документ**

* Внутренний номер и дата
* Контрагент, Номер договора и Грузоотправитель
* Ответственный
* Тип спецификации

![](<../../.gitbook/assets/image (179).png>)

Закладка **Дополнительно**

* Инициатор - кто был инициатор закупки

![](<../../.gitbook/assets/image (396).png>)

Закладка **Способ доставки**

* Условие поставки

![](<../../.gitbook/assets/image (299).png>)

Закладка **Документы**

* Номер документа и дата поставщика
* Условие оплаты

![](<../../.gitbook/assets/image (347).png>)