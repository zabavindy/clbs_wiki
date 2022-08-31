# Расчет APS плана

## Отбор строк MRP

### БО по отбору позиций из MRP BR.MP.MES.IN.COND

Пример:

PLA.KPS1 <> '-' and PLA.KTTOP <> '9999' and PLA.KTTOP <> '9997' and (PLA.KMAT not in ('М00010000000000', 'М00010000000005')) and PLA.KTTOP <> 'RSUP' and (TTMZ.UNTTMZ is null or exists (select 1 from TTMR where TTMZ.UNTTMZ = TTMR.UNTTMZ and TTMR.PR\_UCH > 0))

* PLA.KPS1 <> '-' Берем только учетные операции
* PLA.KTTOP <> '9999' and PLA.KTTOP <> '9997' and PLA.KTTOP <> 'RSUP' - Берем все операции кроме этих
* М00010000000000, М00010000000005 - ресурсы по которым не рассчитывается план

## Методы перед запуском APS планирования

### \_BEFORERF Перед APS-планированием (расчетом номенклатуры)

Определение карт раскроя. Назначение ударов по [Карте переналадки](../../planirovanie-perenaladok/karta-perenadalok.md) из расчет количества назначаемых ударов

```
    var kicksPerWeek = 4900 // Назначаемое количество ударов
```
