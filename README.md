# Yandex.Practicum
Данные проекты были выполнены в ходе обучения в Яндекс.Практикуме, профессии "Специалист по Data Science плюс"

Краткое описание проектов и ссылки:
| |Название|Описание|Инструменты|Сфера деятельности|
|--|----|----|-|----|
|1| [Яндекс.Музыка](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_01.ipynb) | Сравнение данных о прослушивании музыки в Москве и Санкт-Петербурге| `pandas` | `Интернет-сервисы`, `Стриминговый сервис`|
|2| [Кредитный отдел банка](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_02.ipynb) | Анализ признаков влияющих на стоимость квартир в регионе| `pandas`, `pymystem3`, `collections`| Данные максимально сохранены, пропуски заполнены, в том числе с применением случайных величин в диапозоне нормального распределения признаков. По совокупности признаков определены самые близкие к центру квартиры, а также районы с самыми высокими и низкими ценами. Найдена средняя скорость продажи для разных типов недвижимости. Выявлены сезонности в обьеме продаж и колебания цен.|
|3| [Яндекс.Недвижимость](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_03.ipynb) | Анализ статистики использования услуг мобильного оператора клиентами с целью определения приоритетного тарифа для фирмы| `pandas`, `matplotlib` | Для анализа доступен маленький обьем данных. Рассмотрены два тарифных плана нижней и верхней ценовой категории. На основании статистического анализа, выявлены характерные особенности поведения клиентов: затраты, продолжительность использования тарифа, лояльность, стабильность. Проверены гипотезы о поведении клиентов в разных регионах и на разных тарифах. Определен и статичстически подтвержден наиболее выгодный для оператора тариф. |
|4| [Изучения российского проката](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_04.ipynb) | Исследование продаж компьютерных игр в различных регионах и определение стратегии рекламной компании| `pandas`, `matplotlib` | Проведен анализ данных о продажах игр по всему миру начиная с 80-х годов. Определены пики популярности и периоды жизни игровых консолей, а также самые популярные кроссплатформенные игры. Проведен анализ корреляции мнения критиков, журналистов и пользователей с реальными продажами. Составлены портреты клиентов по странам с предпочтениями к платформам, жанрам, конкретным продуктам. Проверены гипотезы о самых популярных жанрах и платформах. |
|5| [Сравнения тарифных планов мобильного оператора](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_05.ipynb) | Модель рекомендаций пользователям альтернативных тарифных планов| `pandas`, `scipy`, `numpy`, `matplotlib`| На основании использования клиентами услуг действующего тарифного плана, настроена модель рекомендации. Использовались RandomForestClassifier, DecisionTreeClassifier, LogisticRegression. Гипермараметры подбирались с помощью кроссвалидации GridSearchCV.| 
|6| [Построение модели для оператора мобильной связи](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_06.ipynb) | Модель для предсказания оттока банковских клиентов| `pandas`, `numpy`, `sklearn`, `enum`, `path`, `urllib.request`| Датасет очищен, признаки кодированы с помощью StandardScaler, использованы RandomForestClassifier, GradientBoostingClassifier, LogisticRegression. Гиперпараметры подобраны кроссвалидацией, применен апсемплинг для устранения дисбаланса классов, для оценки моделей использовалась ROC кривая, F1, accuracy.|
|7| [Отток клиентов из банка](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_07.ipynb) | Модель предсказаний прибыли компании и выбор прибыльных регионов для разработки нефти| `pandas`, `numpy`, `sklearn` |В избранном регионе собраны характеристики для скважин: качество нефти и объём её запасов. Построена модель для предсказания объёма запасов в новых скважинах, использована LinearRegression с метрикой RMSE. Определены скважины с самыми высокими оценками значений добычи. Рассчитаны точки безубыточности, риски убытков, выбран регион с максимальной суммарной прибылью отобранных скважин.|
|8| [Выбор локации для нефтеной скважины](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_08.ipynb) | Модель предсказания качества очистки золотоносной руды| `pandas`, `numpy`, `sklearn` | Проведен анализ корректности расчета исходной эффективности обогащения сырья. Выявлены аномалии в техпроцессе, данные очищены от выбросов. Найдены параметры концентрации металлов на всех этапах очистки, определено влияние размера гранул сырья на процесс обогащения и выхода продукта. Предсказаны параметры процесса по данным о сырье. Использовались: LinearRegression, RandomForestRegressor, Lasso c метрикой SMAPE на кроссвалидации, а также проверкой на константной и Dummy модели.|
|9| [Бизнес модель для отеля](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_09.ipynb) | Алгоритм защиты (обезличивания) персональных данных клиента, и модель предсказание факта выплаты страховой премии| `pandas`, `numpy`, `matplotlib`, `sklearn`, `scipy`, `seaborn`, `catboost` | Подготовленный датасет превращен в матрицу и перемножен на случайную несингулярную обратную квадратную матрицу, с отделением целевого признака. Таким образом выполнено формирование ключа щифрования. На зашифрованном датасете произведены предсказания с использованием LinearRegression с проверкой по коэфициенту детерминации R2. |
|10| [Предсказание стоимости жилья](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_10.ipynb) | Модель предсказания цены подержанных автомобилей| `pandas`, `numpy`, `pyspark` |  Проведен EDA и статанализ, данные очищены от выбросов. Через корреляционную матрицу выявлены важные признаки, лишние признаки удалены. Обучены RandomForestClassifier, CatBoostClassifier, LGBMRegressor, XGboost с подбором параметров с помощью GridSearchCV. Отладка и сравнение по среднеквадратичной ошибке RMSE. |
|11| [Защита персональных данных клиентов](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_11.ipynb) | Модель предсказания заказов такси на следующий час |`pandas`, `numpy`, `matplotlib`, `sklearn`| Проведен анализ времнного ряда по дням в рамках года, определен тренд и сезонность в течении недели и дня. Собрана модель для предсказания на несколько часов вперед в течении дня. Тестировались  SARIMA, XGBoost, CatBoost, GradientBoostingRegressor, LinearRegression метрикой RMSE.|
|12| [Моделирование стоимости автомобилей](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_12.ipynb) | Модель классификации токсичных комментариев| `pandas`, `time`, `sklearn`, `lightgbm` | Данные очищены от разделителей, приведены к регистру, проведена векторизация TfidfVectorizer. Список стопслов загружен из nltk. Параметры подобраны кроссвалидацией, использовалась логистическая регрессия, BERT не использовалась по соображениям экономии ресурсов.|
|13| [Определение температуры звезд](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_13.ipynb) | Статистический анализ спроса на авиабилеты, при проведении музыкальных фестивалей| `pandas`, `seaborn`, `sklearn`, `matplotlib`, `torch` |Проведен статистический анализ данных, проверены гипотезы «Средний спрос на билеты во время фестивалей не отличается от среднего спроса на билеты в обычное время»; «Средний спрос на билеты во время фестивалей отличается от среднего спроса на билеты в обычное время». Пороговое значение alpha 0.05. Для оценки использовался критерий Мынна_Уитни |
|14| [Оценка риска ДТП](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_14.ipynb) | Модель предсказания возраста по фотографии| `pandas`, `numpy`, `matplotlib`, `sklearn`, `lightgbm`, `catboost`, `torch`, `sqlalchemy`  | Модель обучена на обогащенных данных с помощью кроссвалидациина на 10 эпохах на ResNet50 с использованием алгоритма оптимизации Adam(lr=0.0001). Часть данных была обрезана, развернута, сделана ЧБ.|
|15| [Прогноз заказов такси](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_15.ipynb) | Модель оттока клиентов оператора связи| `pandas`, `matplotlib`, `sklearn`, `catboost`, `sqlalchemy`| Проведена очистка данных, балансировка признаков, предотвращена утечка целевого признака. Пропуски заполнены с обогащением датасета новыми фичами. Проведена работа с мултиколлинеарностью. На кроссвалидации CatBoostClassifier удалось получить  ROC-AUC = 0,89.|
|16| [Поиск токсичных комментариев](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_16.ipynb) | Библиотека частых функций | `pandas`, `matplotlib`, `spacy`, `sklearn`, `nltk`, `wordcloud`, `re`, `statsmodels`, `catboost`, `lightgbm`| Собраны функции для разделения выборок, подсчета метрик, кроссвалидации, графики и гистограммы.|
|17| [Определение возраста покупателей](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_17.ipynb) | Библиотека частых функций | `pandas`, `matplotlib`, `keras`| Собраны функции для разделения выборок, подсчета метрик, кроссвалидации, графики и гистограммы.|
|18| [Поиск изображения по запросу](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_18.ipynb) | Библиотека частых функций | `pandas`, `numpy`, `matplotlib`, `sklearn`, `keras`, `sentence_transformers`, `PIL` | Собраны функции для разделения выборок, подсчета метрик, кроссвалидации, графики и гистограммы.|
|19| [Отток клиентов мобильного оператора](https://github.com/Dmitriysind/Yandex.Practicum/blob/main/project_19.ipynb) | Библиотека частых функций | `pandas`, `numpy`, `matplotlib`, `sklearn`, `torch`, `sqlalchemy`, `seaborn`, `skorch`, `catboost`, `phik` | Собраны функции для разделения выборок, подсчета метрик, кроссвалидации, графики и гистограммы.|