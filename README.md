# Анализ каналов привлечения в метрике LTV на 30 день

``` Учебный проект ``` 


## Легенда 

Десктопная игра вышла пару месяцев назад в тестовом режиме на ограниченную аудиторию. Пришла пора оценить, насколько окупаются затраты на маркетинговые активности. Основной канал привлечения — платное продвижение в вебе.

## Цель проекта

Понять, какие каналы привлечения эффективны и неэффективны в метрике LTV, и отследить динамику этой метрики.

## Как посмотреть проект

*Способ 1*

[Ссылка](https://app.powerbi.com/reportEmbed?reportId=537fb358-0991-4a1c-b08c-51ddb389c189&autoAuth=true&ctid=6a4dee01-c3f5-4d4b-bdd2-9e1f1482ac5d)  на проект на app.powerbi.com

*Способ 2*

Скачать файл 3rd_PBI_Cohort_report из репоизитория и открыть непосредственно в Power BI

*Способ 3*

Для ознакомленияя проекта также предоставлены скриншоты ниже


## Дано 

- данные по транзакциям пользователей
- данные по привлечению пользователей (первые сессии пользователей)
- данные о курсе доллара
- данные о затратах на маркетинговые кампании

## Использованные методы
```
- Когортный анализ
- LTV
- Сегментация
```

## Ключевые инструменты
```
- SQL
- Матрицы
- Фильтры
- Условное форматирование 
- Спарклайны
- DAX
```

## Реализация 

![Скриншот анализа LTV по кампаниям, регионам и типам рекламы](/LTV_analisys.png)

![Скриншот реализации LTV по дням](/Dynamics.png)


## Выводы

**№1**

![Скриншот вывода](/Insight.png)

**№2**

В метрике LTV 80% прибыли  приходится на сегмент Россия,  67%  к типу  кампании brand.  Доли Гугл и Яндекс рекламы в метрике LTV приблизительно равны. При сравнении показателей LTV и затраты видно, что их доли в некоторых сегментах несоразмерны.  Так, если 80% всего LTV приходится на сегмент Россия, то и 80%  бюджета тратится на этот сегмент. Напротив, у остальных показателей: 
- 10% LTV при 17% бюджета в сегменте Украина, 
4 и 6% LTV при 1 и 2% бюджета в сегментах Беларусь и Казахстан соответственно,
- 47% LTV при 28% бюджета у Гугл Адвордс,
- 5% LTV при 4% бюджета у РК на конкурентов.

Вследствие появляется гипотеза перераспределения бюджета кампаний:
- Увеличить бюджет РК на сегмент Беларуси, Казахстана, уменьшить сегмент Украины. 
- Продолжать увеличивать долю Гугл Адвордс в бюджете рекламы.
- Увеличить сегмент РК на конкурентов.
