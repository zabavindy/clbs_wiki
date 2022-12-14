---
title: Импорт спецификаций
description: Импорт технологических спецификаций из 1с
published: true
date: 2022-09-08T14:38:22.656Z
tags: 
editor: markdown
dateCreated: 2022-08-31T08:32:11.470Z
---

# Импорт спецификаций

Импорт выполняется автоматически раз в сутки планировщиком \_IMPORTTKSP - Загрузка спецификаций

После импорта могут остаться не обработанные строки спецификаций

>Управление производством > Техническая подготовка производства > Спецификации > Импорт спецификаций

![](<../../assets/image (605).png>)

Возможные причины и пути решения

| Проблема                                        | Описание                                                                                          |
| ----------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| Найдено более одного соответствия изделия       | Выгрузить в Excel и отправить письмом it\_nsi [it\_nsi@rusklimat.ru](mailto:it\_nsi@rusklimat.ru) |
| Не найдено соотвествие кодов ресурса            | Сформировать [заявку на ввод НСИ](../../upravlenie-mdm/zayavki-na-vvod-resursov/)                 |
| Не найдено соотвествия ЕИ изделий               | Выгрузить в Excel и отправить письмом it\_nsi [it\_nsi@rusklimat.ru](mailto:it\_nsi@rusklimat.ru) |
| Не найдено соотвествия ЕИ ресурса               | Выгрузить в Excel и отправить письмом it\_nsi [it\_nsi@rusklimat.ru](mailto:it\_nsi@rusklimat.ru) |
| Не является спецификацией, из списка исключений | По согласованной логике по данным ресурсам спецификации не загружаются                            |

После исправление можно дождаться обработки роботом или выделит необходимые строки и выполнить Импорт из таблицы (F2 -> импорт из таблицы)

![](<../../assets/image (409).png>)

>Выделять необходимо все строки по базовой спецификации

