---
description: Инструкция по использованию журнала работ
---

# Журнал работ

![](<../../../../.gitbook/assets/image (126).png>)

Показываются работы за период:

* если начало выработки или её окончание (TIMENACH\_F, TIMIOKONCH\_F) попадают в период отбора: текущая дата и время - длительность смены

{% hint style="info" %}
Длительность смены указывается либо в БО "BR.MP.SFC.REGISTRATION.PRT.SH", либо 13 часов по умолчанию
{% endhint %}



Правила расцветки:

* если это "Начало" выработки, то карточка белая;
* если это "Окончание выработки" и списание 0%, то карточка красная
* если это "Окончание выработки" и списание >0% и <100%, то карточка жёлтая
* если это "Окончание выработки" и списание 100% (или 100%-допустимый толеранс по настройкам), то карточка зелёная.