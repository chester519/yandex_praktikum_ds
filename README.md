# Проекты Data Science
Репозиторий хранит проекты курса "Data Science", которые я выполнял в ходе обучения на платформе Яндекс.Практикум в течении 2021 - 2022 годов.

Курс позволил мне освоить методы и инструменты, которые применяют специалисты Data Science. Проекты иллюстрируют мои навыки изнания в предметной области, среди них: исследовательский анализ данных, проверка статистических гипотез, очистка данных и выделение признаков, применение машинного обучения для задач классификации и регрессии, нейронных сетей для анализа текстов и компьютерного зрения.

Работы выполнены в среде Jupiter notebook. \
Я применял язык Python 3. \
Основной стек инструментов: `pandas`, `numpy`, `scipy`, `scikit-learn`, `matplotlib`, `seaborn`. В ряде случаев применялись другие библиотеки.

## Исследовательский анализ данных

В этой части я исследовал данные, используя разоичные аналитические методы. Использовал методы обработки пропусков в данных, создания новых признаков, группировки данных в таблицы по нужному признаку. В проектах этой части важную роль играет визуализация данных - наглядное представление графиков и диаграмм. В некоторых проектах я применял методы статистического анализа, чтобы ответить на гипотезы заказчика относительно тех или иных свойств продукта.

| Название проекта | Описание проекта | Инструменты
| :--------------- | :--------------- | :----------
| [Исследование надежности заемщика](https://github.com/IGEremin/yandex_praktikum_ds/tree/main/p01_investigation_of_the_borrowers_creditability) | Исследовал данные клиентов банка. Провел очистку и преобразование данных. С помощью визуализации данных на графиках и групповых таблицах удалось выявить зависимости между надежностью заемщика и рядом параметров, которые можно выявить на этапе одобрения продукта банка. | `pandas` `matplotlib` `pymystem3`
| [Исследование объявлений о продаже недвижимости](https://github.com/IGEremin/yandex_praktikum_ds/tree/main/p02_research_of_ads_for_the_sale_of_apartments) | Анализировал данные объявлений с сервиса Яндекс.Недвижимость. Применил различные методы заполнения пропусков в данных, унифицировал строковые данные, свободно заполняемые пользователем. Обширно использовал визуализацию данных, исследовал распределение признаков и их взаимную корреляцию. В результате удалось установить параметры, оказывающие наибольшее влияние на цену жилья. | `pandas` `matplotlib`
| [Анализ тарифов телеком компании](https://github.com/IGEremin/yandex_praktikum_ds/tree/main/p03_determining_perspective_tariff_for_telecom_company) | Использовал данные об использовании абонентами услуг компании. Провел анализ поведения клиентов в зависимости от используемого тарифа - удалось установит характерные черты пользователей. В результате установил наиболее перспективный тариф для компании, решение обосновал подсчетом выручки. Провел ряд статистических тестов по важным для заказчика вопросам и сформулировал выводы по их результатам. | `pandas` `seaborn` `scipy.stats`
| [Исследование рынка видеоигр](https://github.com/IGEremin/yandex_praktikum_ds/tree/main/p04_research_videogame_market) | Исследовал данные о видеограх за период с 1980 по 2016 год. Использовал различные методы заполнения пропущенных данных, провел исследование зависимости параметров продукта и конечных продаж. Выделил сегменты игр для которых можно ожидать высокие продажи, в зависимости от жанра, платформы и страны выхода на рынок. Также установил ряд других параметров, влияющих на продажи - оценки критиков и прочее. С помощью статистических тестов проверил гипотезы, выдвигаемые заказчиком. | `pandas` `seaborn` `scipy.stats`

## Применение машинного обучения

В дальнейших проектах я применял методы машинного обучения для решения различных задач. Использовал обучение с учителем. В последнем проекте продемонстрировал методы работы с временными рядами.

| Название проекта | Описание проекта | Инструменты
| :--------------- | :--------------- | :----------
| [Рекомендация тарифа телеком компании](https://github.com/IGEremin/yandex_praktikum_ds/tree/main/p05_telecom_tariff_recomendation) | Использовал результаты предыдущего проекта. Решал задачу бинарной классификации. Подобрал наиболее походящий алгоритм машинного обучения для данной задачи, подобрал гиперпараметры, используя кросс-валидацию. Получил предсказательную модель с достаточно высокой точностью, которая способна проанализировать поведение клиента и предложить ему более подходящий тариф. | `pandas` `scikit-learn`
| [Прогнозирование оттока клиентов](https://github.com/IGEremin/yandex_praktikum_ds/tree/main/p06_customer_churn_forecasting) | Решал задачу бинарной классификации с несбалансированными классами. Применял методы балансировки классов - увеличение, уменьшение выборки. Обучил модели случайного леса с подбором гиперпараметров. Исследовал влияние различных методов на метрики точности и полноты предсказаний. В результате удалось получить модель с достаточным качеством. В выводах представил график влияния различных параметров на решения модели, это поможет оценить важность некоторых параметров клиента. | `pandas` `seaborn` `scikit-learn`
| [Определение наилучшей локации для бурения](https://github.com/IGEremin/yandex_praktikum_ds/tree/main/p07_determining_a_favorable_location_for_a_well) | Решал задачу регрессии. По данным заказчика провел экономический расчет бурения скажин. Используя модели линейной регрессии получил предсказания прибыли для разных регионов. Сделал выводы и представил их заказчикам, обосновал выводы расчето прибыли с учетом бурения в регионах. В ходе работы использовал визуализацию данных - графики распределения, матрицы корреляции, для расчета прибыли использовал технику бутстрап.  | `pandas` `seaborn` `scikit-learn`
| [Оценка стоимости автомобиля](https://github.com/IGEremin/yandex_praktikum_ds/tree/main/p09_car_price_estimation) | Решал задачу регрессии. Исследовал набор данных с информацией о продаже автомобилей и их параметрах. Применил различные методы предобработки данных - заполнение средним, заполнение в зависимсоти о других параметров. Применил различные алгоритмы машинного обучения - гребневая регрессия, случайный лес, CatBoost, LightGBM, при обучениииспользовал кросс-валидацию и подобрал гиперпараметры. По важным для заказчика условиям выделил круг моделей, обладающих лучшим качеством. | `pandas` `seaborn` `scikit-learn` `catboost` `lightgbm`
| [Разработка метода защиты персональных данных](https://github.com/IGEremin/yandex_praktikum_ds/tree/main/p08_personal_data_protection) | Разработал метод защиты персональных данных клиента на основе свойств матричного умножения. Привел теоретическое обоснование метода и разработал программный алгоритм шифрования. Показал, что метод не ухудшает предсказания модели линейной регрессии. | `pandas` `numpy` `matplotlib` `scikit-learn`
| [Прогнозирование числа заказов такси](https://github.com/IGEremin/yandex_praktikum_ds/tree/main/p10_taxi_orders_forecasting) | Решал задачу регрессии, используя временной ряд. С помощью методом разложения ряда на компоненты удалось выделить закономерности и тренды заказов такси. Выделил из набора данных новые признаки, такие как скользящее среднее, значения за предыдущие промежутки. Использовал модели линейной регрессии, случайного леса и ансамблевые модели. В результате получил модель, предсказывающую число заказов в будущем, а также сделал выводы о характере изменения целевого признака. | `pandas` `matplotlib` `statsmodels` `scikit-learn` `lightgbm`

## Обработка естественного языка и нейронные сети в задачах компьютерного зрения


| Название проекта | Описание проекта | Инструменты
| :--------------- | :--------------- | :----------
| [Анализ тональности текста](https://github.com/IGEremin/yandex_praktikum_ds/tree/main/p11_sentiment_analysis) | Задача - построить модель, которая выделяет из набора комментариев негативные. В проекте я применил различные методы выделения признаков из текстовых данных: лемматизацию, удаление стоп-слов, векторизацию текста. Использовал разные модели машинного обучения и с помощью кросс-валидации выбрал лучшую модель. | `pandas` `numpy` `nltk` `scikit-learn` `lightgbm`
| [Определение возраста по фотографии](https://github.com/IGEremin/yandex_praktikum_ds/tree/main/p12_age_recognition_by_photo) | Использовал набор данных с размеченными фотографиями лиц людей. С помощью алгоритма ResNet50 получил предсказательную модель. Наглядно показал последовательность обучения модели на новых данных с использованием библиотеки Keras. | `pandas` `matplotlib` `keras`
