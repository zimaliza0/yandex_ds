# 9. Исследование технологического процесса очистки золота

### Задача

Спрогнозировать концентрацию золота при проведении процесса очистки золота

### Описание данных

## Технологический процесс
- Rougher feed — исходное сырье
- Rougher additions (или reagent additions) — флотационные реагенты: Xanthate, Sulphate, Depressant
- Xanthate **— ксантогенат (промотер, или активатор флотации);
- Sulphate — сульфат (на данном производстве сульфид натрия);
- Depressant — депрессант (силикат натрия).
- Rougher process (англ. «грубый процесс») — флотация
- Rougher tails — отвальные хвосты
- Float banks — флотационная установка
- Cleaner process — очистка
- Rougher Au — черновой концентрат золота
- Final Au — финальный концентрат золота  


## Параметры этапов
air amount — объём воздуха
fluid levels — уровень жидкости
feed size — размер гранул сырья
feed rate — скорость подачи  


## Наименование признаков

Наименование признаков формируется по следующему принципу:  

__[этап].[тип_параметра].[название_параметра]__  

Пример: rougher.input.feed_ag

## Возможные значения для блока [этап]
- rougher — флотация
- primary_cleaner — первичная очистка
- secondary_cleaner — вторичная очистка
- final — финальные характеристики  


## Возможные значения для блока [тип_параметра]
- input — параметры сырья
- output — параметры продукта
- state — параметры, характеризующие текущее состояние этапа
- calculation — расчётные характеристики

## Целевые признаки
- эффективность обогащения чернового концентрата rougher.output.recovery;
- эффективность обогащения финального концентрата final.output.recovery.

### Инструменты

`машинное обучение`, `sklearn`, `seaborn`, `matplotlib`, `numpy`, `pandas`