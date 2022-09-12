---
title: Пакеты экспорта LV
description: 
published: true
date: 2022-09-11T17:31:41.313Z
tags: 
editor: markdown
dateCreated: 2022-08-31T09:15:40.634Z
---

# Пакеты экспорта LV

## Типы процессов

* [Поступление товаров и услуг](../../../../uchet/postuplenie-tovarov-i-uslug/) - пакет RECEIPT (наряд на приемку)
* [Внутреннее перемещение](../../../../uchet/peremesheniya-tovarov-1/vnutrennee-peremeshenie/), [Выдача и возврат из эксплуатации](../../../../uchet/peremesheniya-tovarov-1/materialy-v-ekspluatacii/), [Выдача со списание](../../../../uchet/peremesheniya-tovarov-1/untitled/) - пакет ORDER (при получении от LV), RECEIPT (при сдаче на склад)
* [Передача и возврат с ответ хранение](../../../../uchet/otvet-khranenie/) - пакет ORDER (при получении от LV), RECEIPT (при сдаче на склад)
* [Сдача продукции на СГП](../../../../uchet/otgruzka-produkcii/sdacha-produkcii-na-sgp-1.md) - пакет [RELOCATE\_2](relocate\_2.md) (наряд на перемещение)
* [Реализация ТМЦ](../../../../uchet/realizaciya/realizaciya-tmc.md) -пакет ORDER (при получении от LV)
* [Возврат ТМЦ поставщику](../../../../uchet/vozvrat-tovarov-i-uslug/untitled-1.md) - пакет ORDER (при получении от LV)
* [Передача материалов кооператору](../../../../uchet/kooperaciya/poluchenie-uslug/untitled-2.md) - пакет ORDER (при получении от LV)

## Условие выгрузки

* Документ попадет на стадии Экспорт LV и Импорт LV если у подразделения Отправителя и Получателя признак ZEX3 не пустой
* Справочник SPR = PD2
  * База LV определяется по полю NAIM/NAIM\_S
  * Идентификатор номенклатуры для выгрузки определяется по полюCHAR\_SPA

| Код | Наименование |
| --- | ------------ |
| 0   | Код LV       |
| 1   | Код ЕС НСИ   |
| 2   | Код 1С       |
| 3   | Guid 1C      |
