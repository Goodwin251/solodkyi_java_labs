﻿# [Лабораторна робота 7](https://github.com/Goodwin251/solodkyi_java_labs/blob/main/README.md)

Зробив Солодкий Ярослав Тарасович з групи ПД-32

## Мета

Навчити студентів ефективно використовувати Java Streams для аналізу даних, отриманих через HTTP-запити. Студенти будуть взаємодіяти з реальним API для отримання метеорологічних даних.

## Завдання

1. Взаємодія з API
	* Виконайте HTTP-запит до метеорологічного API для отримання даних.
	* Обробіть отримані дані і перетворіть їх у потрібний формат.
1. Аналіз екстремальних погодних умов
	* Знайдіть 10 найгарячіших та найхолодніших станцій за середньою температурою.
	* Знайдіть 10 найвологіших станцій за середнім рівнем опадів.
1. Розпізнавання патернів
	* Визначте станції, на яких було більше 7 послідовних днів опадів.
	* Визначте станції, на яких температура зросла на щонайменше 5°C протягом 5 послідовних днів.
1. Агрегація та підсумкова статистика
	* Розрахуйте середню глобальну температуру, вологість та рівень опадів для кожного місяця.
	* Визначте місяць з найвищою середньою швидкістю вітру.
1. Відображення результатів
	* Представте аналізовані дані користувачу у вигляді таблиці або графіка.

## Формат прийняття лабораторної роботи: 

1. Робота повинна мати план розробки програми та послідовність виконаних дій.
1. Код розробленого додатку прикріпити у вигляді посилання на GitHub.
1. GitHub повинен мати комміти як ви зробили на протязі розробки програми. Мова коммітів: Англійська.

## План розробки

1. Виконати HTTP-запит до метеорологічного API для отримання даних.
1. Обробіть отримані дані і перетворіть їх у прийнятний формат.
1. Відобразити їх у консольній таблиці.
1. Створити тестові класи, де промоделювати різні сценарії для тестування обробки виняткових ситуацій.
1. Зібрати білд з Maven, щоб перевірити вірність виконання тестів.
1. Залити лабораторну роботу на репозиторій на гітхабі.

## Тести

### [WeatherAPIClientTest.java](https://github.com/Goodwin251/solodkyi_java_labs/blob/main/src/test/java/com/solodkyi/java_labs/Lab8Test/WeatherAPIClientTest.java)
	* testCorrectURL - створення коректного URL;
	* testInCorrectURL - неправильне створення URL;
	* testCorrectConnection - перевірка правильного під'єднання;
	* testGetIOExceptionWhileConnect - вибиття помилки GetIOException при під'єднанні;
	* testCreateBufferReader - перевірка створення BufferReader.