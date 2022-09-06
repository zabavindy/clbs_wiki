---
description: Инструкция по формированию спецификации на оказание услуг
---

# Спецификации на услуги (оказанные)

Встаньте на документ «Заказ покупателя (ЗП)» и нажмите «F2 – Создать спецификацию на услугу»

![](<../../../.gitbook/assets/0 (46).png>)

{% hint style="info" %}
Заказ должен быть со статусом код 6 - Заказ на услуги
{% endhint %}

![](<../../../.gitbook/assets/1 (37).png>)

Если заказ не является заказом на услугу, то выйдет сообщение, и спецификация на услугу не сформируется:

![](<../../../.gitbook/assets/2 (29).png>)

В появившемся окне поля «Организация» и «Договор» установлены по умолчанию из документа «Заказ покупателя» и являются не редактируемыми. Добавьте услуги. Для добавления услуг нажмите кнопку «Добавить»:

![](<../../../.gitbook/assets/3 (58).png>)

В появившемся окне добавьте услуги. Введите услугу, количество, цену и нажмите «ОК»:

![](<../../../.gitbook/assets/4 (57).png>)

Если услуг несколько, то добавьте аналогично кнопкой «Добавить» (п.2-3).

Когда все услуги добавлены, нажмите кнопку «Ок»:

![](<../../../.gitbook/assets/5 (20).png>)

К документу будет создан документ на услуги.

Для просмотра привязанного документа «Спецификация на услугу» нажмите «F12 – Привязки – Связанные документы»:

![](<../../../.gitbook/assets/6 (24).png>)

![](<../../../.gitbook/assets/7 (15).png>)

Далее, спецификацию на услуги нужно выгрузить в 1С. Для этого переведите документ на стадию «Экспорт1С», нажав кнопку «Передать вперед»:

![](<../../../.gitbook/assets/8 (5).png>)

Документ перейдет на стадию «Экспорт 1С»

Когда сформируется пакет экспорта в 1С, то документ автоматически перейдет на стадию «Обработка 1С».

Когда загрузится документ импорта с номером спецификации в 1С бухгалтерии, документ автоматически перейдет на стадию «Архив».