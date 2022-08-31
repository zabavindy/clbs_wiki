# Обработка в 1с

## Обработки в 1с

* ИЗТТ - \\\rusklimat.ru\app\1C\_Exchange\UPP\IZTT\ITEnt\Обработка\ОбменITEnt.epf
* РТ и ТК - \\\rusklimat.ru\app\1C\_Exchange\UPP\RT\ITEnt\Обработка\ОбменITEnt.epf
* ВКО - \\\rusklimat.ru\app\1C\_Exchange\UPP\VKO\ITEnt\Обработка\ОбменITEnt.epf

## Описание потоков

### Номенклатуры

{% hint style="info" %}
Выгрузка из IT-Ent -> 1с
{% endhint %}

Для готовой продукции ИЗТТ (группа G) при добавлении значений фасет R29, R30, R37 необходимо настраивать Cправочник стыковки ресурсов IT Ent в базе 1с

![](<../../.gitbook/assets/image (801).png>)

[Выгружается в пакет](pakety-v-it-enterprise/) - KSM

### Складов и подразделения

{% hint style="info" %}
Выгрузка из 1с -> IT-Ent. Склады автоматически не попадают на выгрузку в IT-Ent
{% endhint %}

Их нужно либо зарегистрировать в плане обмена EAM – «IT Enterprise», либо добавить в регистр сведений «Стек обмена IT Ent.»

[Выгружается в пакет](pakety-v-it-enterprise/) - POD

### Персонала

{% hint style="info" %}
Выгрузка из 1с -> IT-Ent
{% endhint %}

Выгрузка формируется на основании документов в 1с: Прием на работу, Увольнение, Кадровые перемещения

{% hint style="info" %}
При выгрузке пакета по увольнению пользователь в IT-Enterprise **блокируется**
{% endhint %}

[Выгружается в пакет](pakety-v-it-enterprise/) - [KDK](pakety-v-it-enterprise/#kdk-spravochnik-personal)

### Контрагенты

{% hint style="info" %}
Выгрузка из IT-Ent -> 1с
{% endhint %}

[Выгружается в пакет](pakety-v-it-enterprise/) - ORG

### Договора

{% hint style="info" %}
Выгрузка из IT-Ent -> 1с
{% endhint %}

[Выгружается в пакет](pakety-v-it-enterprise/) - DOG

### Справочники статей затрат

[Выгружается в пакет](pakety-v-it-enterprise/) - KAU

### Календарные планы (платежи)

{% hint style="info" %}
Выгрузка из IT-Ent -> 1с
{% endhint %}

[Выгружается в пакет](pakety-v-it-enterprise/) - DMZK

### Документы движения

{% hint style="info" %}
Выгрузка из IT-Ent -> 1с
{% endhint %}

[Выгружается в пакет](pakety-v-it-enterprise/)
