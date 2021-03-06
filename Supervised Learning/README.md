
## Прогнозирование оттока клиентов банка

### Набор инструментов
Работа с дисбалансом классов;  
Изучение и применение метрик классификации (f1, ROC-AUC, confusion matrix);  
Изучение и применение метрик регрессии (RMSE, MAE, R2).

### Вводные данные
Из банка стали уходить клиенты. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.

### Цель
Необходимо создать модель и спрогнозировать, уйдёт клиент из банка в ближайшее время или нет.
В наличии исторические данные о поведении клиентов и расторжении договоров с банком.

### Структура проекта  

1. Изучение подготовка данных к анализу; 
2. Исследование баланса классов, обучение модели без учёта дисбаланса;
3. Улучшение качества модели с учетом дисбаланс классов. Обучение различных модели и выбор лучшей;
4. Проверка модели на тестовых данных;
5. Проверим модели на вменяемость. 

### Общий вывод  

В данном исследовании проведена работа по созданию модели классификации клиентов банка «Бета-Банк» на тех, которые останутся в банке и тех, которые уйдут из банка в ближайшей перспективе. 
Основными задачами исследования были создание модели с определенным уровнем показателя f1, применение методов балансировки классов целевого признака и тестирование нескольких различных моделей.

Основные выводы, полученные после выполнения работы:  
1. Перед нами был пример задачи классификации; 
2. Для улучшения результатов работы моделей была проведена балансировка классов;  
3. Первичное тестирование моделей без учета баланса классов продемонстрировало следующие показатели:   
4. Были построены модели на основе трех алгоритмов - Решающее дерево, Случайный лес и алгоритм Логистической регрессии;
5. Наилучший результат на увеличенной и уменьшенной выборках показала модель Случайного леса;
6. На тестовой выборке данная модель показала знаение f1-меры - 0.61, а метрика AUC-ROC оказалась равна 0.85;
