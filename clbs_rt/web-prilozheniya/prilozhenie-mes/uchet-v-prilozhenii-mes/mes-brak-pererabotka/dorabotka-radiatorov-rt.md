---
title: Переработка АБР УДП
description: Инструкция по доработке радиаторов на участке доработки продукции (РТ)
published: true
date: 2022-09-11T17:31:41.313Z
tags: 
editor: markdown
dateCreated: 2022-08-31T09:15:40.634Z
---

# Переработка АБР УДП

## Разукомплектация

На участок доработки приходят радиаторы с талоном «неокончательный брак». Чтобы взять талон в работу необходимо в программе MES зайти в меню «Переработка АБР УДП»

![](<../../../../assets/0 (54)1.png>)

Откроется меню, в котором для начала работы необходимо отсканировать или ввести QR-код талона. Далее, нажать кнопку «Получить описание задания»

![](<../../../../assets/1 (64)1.png>)

После этого, в строках ниже отобразится информация о количестве радиаторов и общем количестве секций в них. Далее необходимо нажать кнопку «Разукомплектовать» и приступить к работе, согласно стандартным процедурам. В результате на участок поступит соответствующее количество секций

## Выработка годных

На вкладке «Выработка годных радиаторов» можно зафиксировать факт сборки годных радиаторов из секций, которые числятся в остатках участка доработки

![](<../../../../assets/2 (7)1.png>)

Для этого из выпадающего списка выбирается модель радиатора, секционность и вводится количество радиаторов. В информационных полях справа показывается остаток секций данного типа в подразделении и максимальное количество радиаторов, которые можно собрать из этих секций

Далее указываются дефекты входящих секций, которые были исправлены. Дефекты можно добавлять или удалять из таблицы нажатием на соответствующие кнопки справа и снизу

После этого надо нажать кнопку «Зарегистрировать выработку». Будет создан документ Акт выработки и напечатан ярлык новой партии

## Списание брака

На вкладке «Списание бракованных секций» выбирается тип секции из остатков на участке, вводится количество и заполняется список дефектов на этих секциях. В информационном поле справа показывается общий остаток выбранных секций на участке, доступный к списанию

![](<../../../../assets/3 (3)1.png>)

По нажатию кнопки «Зарегистрировать списание» создается документ Акт возникновения окончательного брака и печатается ярлык партии

## Журнал выработки

На вкладке «Журнал выработки» можно просмотреть всю зарегистрированную выработку годных радиаторов за текущую смену. Для этого надо нажать кнопку «Обновить», отобразится список документов выработки

>При необходимости можно повторно напечатать ярлык по документу, нажав на соответствующую кнопку печати ярлыка


![](<../../../../assets/4 (6)1.png>)
