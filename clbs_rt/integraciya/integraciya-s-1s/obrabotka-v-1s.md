---
title: Обработка в 1с
description: 
published: true
date: 2022-09-11T17:31:41.313Z
tags: 
editor: markdown
dateCreated: 2022-08-31T09:15:40.634Z
---

# Обработка в 1с

## Обработки в 1с

* ИЗТТ - \\\rusklimat.ru\app\1C\_Exchange\UPP\IZTT\ITEnt\Обработка\ОбменITEnt.epf
* РТ и ТК - \\\rusklimat.ru\app\1C\_Exchange\UPP\RT\ITEnt\Обработка\ОбменITEnt.epf
* ВКО - \\\rusklimat.ru\app\1C\_Exchange\UPP\VKO\ITEnt\Обработка\ОбменITEnt.epf

## Описание потоков

### Номенклатуры

>Выгрузка из IT-Ent -> 1с

Для готовой продукции ИЗТТ (группа G) при добавлении значений фасет R29, R30, R37 необходимо настраивать Cправочник стыковки ресурсов IT Ent в базе 1с

![](<../../assets/image (801).png>)

[Выгружается в пакет](pakety-v-it-enterprise/) - KSM

### Складов и подразделения

>Выгрузка из 1с -> IT-Ent. Склады автоматически не попадают на выгрузку в IT-Ent

Их нужно либо зарегистрировать в плане обмена EAM – «IT Enterprise», либо добавить в регистр сведений «Стек обмена IT Ent.»

[Выгружается в пакет](pakety-v-it-enterprise/) - POD

### Персонала

>Выгрузка из 1с -> IT-Ent

Выгрузка формируется на основании документов в 1с: Прием на работу, Увольнение, Кадровые перемещения


>При выгрузке пакета по увольнению пользователь в IT-Enterprise **блокируется**

[Выгружается в пакет](pakety-v-it-enterprise/) - [KDK](pakety-v-it-enterprise/#kdk-spravochnik-personal)

### Контрагенты

>Выгрузка из IT-Ent -> 1с

[Выгружается в пакет](pakety-v-it-enterprise/) - ORG

### Договора

>Выгрузка из IT-Ent -> 1с

[Выгружается в пакет](pakety-v-it-enterprise/) - DOG

### Справочники статей затрат

[Выгружается в пакет](pakety-v-it-enterprise/) - KAU

### Календарные планы (платежи)

>Выгрузка из IT-Ent -> 1с

[Выгружается в пакет](pakety-v-it-enterprise/) - DMZK

### Документы движения

>Выгрузка из IT-Ent -> 1с

[Выгружается в пакет](pakety-v-it-enterprise/)
