
## Опредедение возраста человека по фотографии
### Набор инструментов
Библиотека keras: применение базовых CNN, архитекур LeNet и ResNet.
Тестирование различных методов аугментации изображений.
### Вводные данные
Крупный супермаркет внедряет систему компьютерного зрения для обработки фотографий покупателей.
Модель поможет определять возраст клиентов, чтобы:
* Анализировать покупки и предлагать товары, которые могут заинтересовать покупателей этой возрастной группы;
* Контролировать добросовестность кассиров при продаже алкоголя.
* Необходимо построить модель, которая по фотографии определит приблизительный возраст человека.
В нашем распоряжении набор фотографий людей с указанием возраста.

### Цель

Построить модель, которая по фотографии определит приблизительный возраст человека. Метрика MAE не должна превысить 8 пунктов.

### Структура проекта
1. Проанализировать имеющиеся данные: количество фотографий, размер, возрастные группы;
2. Подготовить данные: создать datagen'ы, скалировать и провести аугментацию;
3. Создать и обучить нейронную сеть. Протестировать различные архитектуры. Рассчитать качество модели.  

### Общий вывод 
Цель исследования выполнена: обученная модель демонстрирует показатель MAE = 6.74 с горизонтальным отражением фотографий.
Исходные данные содержали 7.5 тысяч записей, без пропусков и выбросов. Большинство людей на фотографиях запечетлено в возрастном диапазоне 20-30 лет. Финальная модель содержит архитектуру ResNet и предобученные на ImageNet сверточные слои.  

#### *Важно*
Обучение модели происходило на отдельном учебном сервере. В случае получения результата, удовлетворяющего условиям задания, повторно запустить проект было невозможно. Поэтому представлен код первого удачного запуска.


```python

```