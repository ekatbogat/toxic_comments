Проект: Классификация токсичных комментариев
1. Контекст проекта:
Заказчик: Интернет-магазин.
Цель проекта: Разработать инструмент для выявления токсичных комментариев среди предложенных правок и отправки их на модерацию.
2. Исследование данных:
Исходные данные: Файл toxic_comments.csv с текстами комментариев и меткой токсичности.
Характеристики данных:
159292 строки.
Без дубликатов и пропусков.
Тексты комментариев были очищены и лемматизированы. 
Бинарная классификация: 89.8% комментариев токсичны.
4. Подготовка данных:
Оставлены столбцы toxic и text.
Используется классификация на позитивные (1) и негативные (0) комментарии.
5. Разделение выборок:
6. Проверка соотношения классов показала, что в датасете имеет место явный дисбаланс. Мажорный класс составляет лишь 10% от всего датасета. После векторизации датасет образовал матрицу размером (119469, 134385). В итоге полученный датасет разделен на обучающую 90 % и тестовые выборки 10 %.
7. Обучение моделей:
Модели:
Логистическая регрессия: F1 = 0.76.
Решающее дерево: F1 = 0.58.
Случайный лес: F1 = 0.66.
Выбор модели:
Логистическая регрессия с F1 = 0.76 лучшая.
8. Тестирование модели:
Модель LogisticRegression на тестовой выборке: F1 = 0.78.
9. Общий вывод:
Разработана модель для классификации токсичных комментариев.
Наилучший результат показала логистическая регрессия.
Метрика F1 на тесте достигла значения 0.78, что соответствует требованию заказчика (F1 не меньше 0.75).
Рекомендации по дальнейшему развитию: дополнительная настройка модели, мониторинг новых данных для постоянной актуальности.



