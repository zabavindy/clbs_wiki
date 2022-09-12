---
title: Пакеты импорта 1с
description: 
published: true
date: 2022-09-11T17:31:41.313Z
tags: 
editor: markdown
dateCreated: 2022-08-31T09:15:40.634Z
---

# Пакеты импорта 1с

SQL таблицы:

* IMPDZ - Заголовок пакета
* IMPDS - Строки пакета



>Для создания заголовка пакета импорта необходимо использовать хранимую процедуру, которая возвращает код записи IMPDZ, по которой потом нужно вставлять строки IMPDS


Параметры запуска кода для вставки заголовка пакета импорта из 1с

* Command    = Новый COMОбъект("ADODB.Command");
* Command.ActiveConnection   = Connection;
* Command.CommandTimeout = 30;
* Command.CommandType = 4
* Command.Prepared = true;
* Command.NamedParameters = true;

&#x20;

&#x20;Команда вставки

* Command.CommandText = " | INSERT\_IMPDZ";
* Command.Parameters.Append(Command.CreateParameter("@KPROF",129,1,50,"1С"));
* Command.Parameters.Append(Command.CreateParameter("@CONTENT",129,1,50,CONTENT));
  * CONTENT = 'DMZ\_1C'
* Command.Parameters.Append(Command.CreateParameter("@SENDER",129,1,50,ТекReceiver));
  * ТекReceiver = '00001'  - РоялТермо
  * ТекReceiver = '00005' - Термокомпонент
* Command.Parameters.Append(Command.CreateParameter("@RECEIVER",129,1,50,"IT-Enterprise"));
* Command.Parameters.Append(Command.CreateParameter("@FIO\_D",129,1,50,"iztt2"));
* Command.Parameters.Append(Command.CreateParameter("@RESULT",2,1,5,1));

&#x20;Список пакетов

* [KDK ](kdk.md#kdk-spravochnik-personal)- [Справочник персонал](../../../../human-resources/nsi-hr/spravochnik-personala.md)
* [DMZ\_1C](dmz\_1c.md) - Импорт данных по документам выгруженным из IT в 1с
