
## Определение цены автомобиля по имеющимся характеристикам

### Набор инструментов

Предобработка данных: обработка пропусков и дубликатов, изменение типа данных, группировка таблиц;  
Применение стандартных моделей прогнозирования и моделей градиентного бустинга: sklearn, LigtGBM, XGBoost, CatBoost;  
Проверка результатов на валидационной и тестовых выборках.
### Вводные данные
В данном проекте стоит задача построить модель для определения стоимости автомобиля для сервиса по продаже автомобилей с пробегом, который разрабатывает приложение для привлечения новых клиентов. В распоряжении есть следующие данные: технические характеристики, комплектации и цены автомобилей.
Заказчику важны:
* качество предсказания;
* скорость предсказания;
* время обучения.  

### Цель 
Создание модели, которая предсказывает цену автомобиля на основании определенных принаков.
Имеются размеченные данные: характеристики автомобилей и цена продажи.  

### Структура проекта 
1. Загрузка и обработка данных: заполнение пропусков, группировка по признакам, поиск дубликатов, визуализация результатов;
2. Обучение моделей градиентного бустинга, анализ скорости обучения;
3. Обучение моделей прогнозирования, требующих dummy-преобразования - линейная регрессия, случайный лес.
4. Валидация моделей и выбор лучшей.  

### Общий вывод  
В исследовании приняли участие 5 моделей : 'LightGBM', 'Catboost', 'Gradient_Boosting', 'LinearRegression', 'RandomForestRegressor'  
Основной метрикой тестрирования стала метрика RMSE.
На первом этапе исследования был произведен анализ данных и заполнены пропущенные значения.
На втором этапе работы было протестировано 5 моделей прогнозирования. 
Наилучшей и рекомендованной к использованию моделью признана LightGBM - со значением RMSE на тестовой выборке = 1654.23,  временем обучения = 1,5 минуты, временем предсказания 10 сек на учебном сервере.
