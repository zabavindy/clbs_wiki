# Подразделения

{% hint style="info" %}
Администрирование системы → Управление основными данными (MDM) → Основные справочники → Подразделения → Справочник подразделений
{% endhint %}

![](<../../.gitbook/assets/image (42).png>)

## Типы иерархий

**IT\_СТРУКТ** - единая структура холдинга Руклимат

Под каждый объект создается отдельная иерархия

| Код символьный | Наименование   |
| -------------- | -------------- |
| 1C\_IZTT       | Структура ИЗТТ |
| 1C\_RT         | Структура РТ   |
| 1C\_TK         | Структура TK   |
| 1C\_VKO        | Структура VKO  |
| BIG            | Структура BIG  |

## Справочник подразделений

### Закладка Подразделение

![](<../../.gitbook/assets/image (985).png>)

* Объекты
* Действует с/по
* Ввод документов до
* Тип подразделения
* Центр финансового учета
* Доп. признак 1 - Площадка. используется для разделения учета, доступа и т.д. внутри объекта
* Доп. признак 2 - [Выбор базы для интеграции с LV](../../integraciya/integraciya-s-lv/)
* Доп. признак 3 - [Вид документа для выдачи материалов в подразделение](../../uchet/peremesheniya-tovarov-1/)
* Обозначения
* Наименования
* Руководитель
* МОЛ по ТМЦ - Основной МОЛ по подразделению при формировании документов учета
* Подразделение для анализа - Проставляется для подразделений по которым необходимо разделить объект

### Закладка Дополнительные параметры

![](<../../.gitbook/assets/image (780).png>)

* "Старый" код 3 - [Признак интеграции с LV](../../integraciya/integraciya-s-lv/)

### Закладка Техническая подготовка

![](<../../.gitbook/assets/image (190).png>)

* Учетная точка -&#x20;
* Участвует в расцеховке - [Только эти подразделения возможно выбрать при создании операции техмаршрута](../../pdm/pdm-tpp/tekhnologicheskaya-podgotovka-proizvodstva/sozdanie-tekhprocessa/sozdanie-operacii.md)