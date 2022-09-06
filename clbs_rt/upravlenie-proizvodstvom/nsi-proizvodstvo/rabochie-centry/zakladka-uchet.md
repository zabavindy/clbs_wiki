---
description: Описание настроек учета по рабочему центры
---

# Закладка Учет

## Выработка

![](<../../../.gitbook/assets/image (908).png>)

* Очередь обработки событий - 1,2, ... внутри одной группы параллельная обработка (расценка) актов выработки
* Создавать партию годного в момент взятия задания в работу - Применяется для регистрации показателей качества в [приложении MES](../../../web-prilozheniya/prilozhenie-mes/uchet-v-prilozhenii-mes/mes-kachestvo/zanesenie-parametrov-mezhoperacionnogo-kontrolya-v-mes.md)
* Регистрация выработке под заказ "Свободное наличие" - Регистрация выработки производится на свободный заказ (MTS). Обнуляется заказ кредит у строк списания материалов
* Правило формирования смены для выработки
  * По фиксации за рабочим центром - По дате и времени регистрации в приложении MES
  * По времени регистрации выработки - По дате и времени фиксации выработки
* **При регистрации начала выработки проверять наличие всех материалов, п/ф для изготовления** - проверка наличия установленных материалов при взятии в работу задания;
* **При регистрации окончания / частично проверять прогресс списания** - контроль полноты списания при выработке задания;

## Списание

![](<../../../.gitbook/assets/image (633).png>)

* Максимальный % автоматического выполнения экономии/перерасхода – установленное значение на которое разрешены экономия или перерасход от нормы входящего материала, при выполнении списания в мобильном приложении MES. Данный параметр автоматически устанавливает признаки: «Изготовлено все» - для экономии или «Использовано все» - для перерасхода. Значение данного параметра должно быть < или = значению указанному в параметре «Максимально-допустимый % экономии/перерасхода». Считается если установлен признак "Автоматически определять перерасход"
* Автоматически определять перерасход
* Снимать партию материала с рабочего центра после списания – при установленном признаке после выполнения списания в мобильном приложении MES все установленные партии на рабочем центре автоматически снимаются. При следующем входе в производственное задание необходимо повторно выполнить установку партий входящих материалов

## Отходы

![](<../../../.gitbook/assets/image (369).png>)

## Печать

![](<../../../.gitbook/assets/image (856).png>)

* Ближайший принтер – выбирается из выпадающего списка или справочника принтеров по кнопке На указанном в параметре принтере будут печататься бирки на произведенные изделия, использованные материалы, полученные отходы
* Форма бирки на годную продукцию – выбирается из выпадающего списка или справочника печатных форм ярлыков
* Форма бирки на продукцию с исправленным браком – выбирается из выпадающего списка или справочника печатных форм ярлыков
* Форма бирки на продукцию с окончательным браком – выбирается из выпадающего списка или справочника печатных форм ярлыков
* Форма бирки на отходы – выбирается из выпадающего списка или справочника печатных форм ярлыков

## Общие

![](<../../../.gitbook/assets/image (226).png>)

* Центр учета – виртуальный РЦ для объединения производственных заданий (на разные РЦ) в общий список. Выбранное значение используется для отображения производственных заданий в веб-приложении MES. Выбирается из выпадающего списка или справочника рабочих центров . Виртуальный РЦ не используется в планировании&#x20;
* Количество допустимых к взятию в работу заданий – заданное значение определяет количество производственных заданий для выполнения в мобильном приложении MES. Количество производственных заданий в данном параметре не должно превышать количество, указанное в бизнес- объекте BR.MP.SFC.ST.CREATION.TCNT
* Скрыть кнопку "Установить материалы" в web приложении MES
* Автоматическая регистрация начала выработки по незавершенному заданию - автоматическая регистрация начала выработки после выработки задания с оставшимся количеством больше 0
* Фиксация простоев с учетом технического места - При фиксации простоев детализация до технического места
* Форма корректировки события регистрации выработки из журнала работ для веб-приложений - выбор формы для доп функций ([Повторная печать ярлыка](../../../web-prilozheniya/prilozhenie-mes/uchet-v-prilozhenii-mes/mes-vyrabotka/ustanovka-partii-materialov.md#pechat), [Распределение остатков на выработку](../../../web-prilozheniya/prilozhenie-mes/uchet-v-prilozhenii-mes/mes-vyrabotka/ustanovka-partii-materialov.md#snyat-s-raspredeleniem-na-vypusk))