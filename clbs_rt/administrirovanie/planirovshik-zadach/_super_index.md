---
title: _SUPER_INDEX
description: 
published: true
date: 2022-08-29T09:02:42.934Z
tags: 
editor: markdown
dateCreated: 2022-08-29T08:44:45.264Z
---
# \_SUPER\_INDEX

Для высоконагруженных баз Reorganize является более предпочтительным чем Rebuild потому что не вызывает блокировок

[https://docs.microsoft.com/ru-ru/sql/relational-databases/indexes/reorganize-and-rebuild-indexes?view=sql-server-ver15](https://docs.microsoft.com/ru-ru/sql/relational-databases/indexes/reorganize-and-rebuild-indexes?view=sql-server-ver15)

![](<../../assets/0 (80)1.png>)

Работа робота разбита на 3 этапа (приоритета)

* Этап 1. Таблицы "DMS", "DMZ", "CLCR", "\_CLCRFAD", "CLCH", "\_STOCKEX","PLA" – HardCode
* Этап 2. Таблицы из описания БД (Таблица DBN), за исключением таблиц из пункта 1)

Далее проверяется фрагментация индекса и в соответствии с рекомендациями майкрософт , если она более 10% то выполняется Reorganize индекса.

* Этап 3. Подобие второго прохода. Сложным запросом использующим системные функции и таблицы, мы выбираем все индексы в БД, где фрагментация более 10%. (Следует отметить, что за время работы 1) и 2) часть индексов уже могли “испортится”, данный запрос в таком случае их тоже возьмет в работу.

Собственно для каждой записи выполняется Reorganize

>**Важно**: для исключения коллизий, робот объединен в одну группу с системным планировщиком INDEX\_DEFRAGMENTATION\_DOCUMENTS, что обеспечивает поочередный запуск планировщиков

