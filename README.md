# Тестовое задание QA Intern в Mindbox:
### Вопрос 1
Есть форма на сайте, которая рассчитывает возможность оформления паспорта РФ в зависимости
от возраста (по действующему законодательству). Поле принимает на вход целые числа от 0 до
115 включительно. В результате получаем сообщение: “Нельзя оформить”, “Можно оформить” или
“Ошибка”.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Разбейте входные данные по технике граничных значений и определите результат для каждого
случая<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• Разбейте входные данные на классы эквивалентности, приведите пример входного значения
для каждого класса и укажите результат<br>


### Ответ

Таблица КЭ и ГЗ форма оформления паспорта РФ

|Группа проверок|Название класса|Тип класса|Границы|Тестовые данные внутри класса|Тестовые данные на границах|Пояснение и оптимизация|Результат|
|:-|:---------|:------|:--------------|:-------------|:--------|:-------|:------|
| |	диапазон |	00\:01, 08\:00 |	04\:00 |	00\:01, 00\:02, 07\:59, 08\:00 |	Скорость автомобиля 45 км/ч|
 |	диапазон |	08\:01, 12\:00 |	10\:00 |	08\:01, 08\:02, 11\:59, 12\:00 |	Скорость автомобиля 30 км/ч|
| |	диапазон |	12\:01, 18\:00 |	15\:00 |	12\:01, 12\:02, 17\:59, 18\:00 |	Скорость автомобиля 40 км/ч|
|18\:01-22:00 |	диапазон |	18\:01, 22\:00 |	20\:00 |	18\:01, 18\:02, 21\:59, 22\:00 |	Скорость автомобиля 25 км/ч|
|22\:01-00:00 |	диапазон |	22\:01, 00\:00 |	23\:00 |	22\:01, 22\:02, 23\:59, 00\:00 |	Скорость автомобиля 45 км/ч|
