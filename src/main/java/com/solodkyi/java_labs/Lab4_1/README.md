﻿# [Лабораторна робота 4_1](https://github.com/Goodwin251/solodkyi_java_labs/blob/main/README.md)

Зробив Солодкий Ярослав Тарасович з групи ПД-32

## Завдання

1. Реалізуйте функцію, яка перевіряє, чи дане слово є паліндромом (читається так само, як назад, так і вперед), використовуючи рядки Java. 
1. Покрити тестами функціональність програми.

## Формат прийняття лабораторної роботи: 

1. Робота повинна мати план розробки програми та послідовність виконаних дій.
1. Код розробленого додатку прикріпити у вигляді посилання на GitHub
1. GitHub повинен мати комміти як ви зробили на протязі розробки програми. Мова коммітів: Англійська

## План розробки

1. Зробити метод IsPalindromeTest для перевірки слів на наявність цієї властивості.
1. Викликати в main декілька разів метод для демонстрації його роботи.
1. Зробити тест для перевірки працездатності метода з юніт тестами.
1. Зібрати білд з Maven, щоб перевірити вірність виконання тестів.
1. Залити лабораторну роботу на репозиторій на гітхабі.

## Тести

### [IsPalindromeTest.java](https://github.com/Goodwin251/solodkyi_java_labs/blob/main/src/test/java/com/solodkyi/java_labs/Lab4_1Test/IsPalindromeTest.java)
	* testPalindromes - метод перевіряє паліндроми;
	* testIsNotPalindromes - метод перевіряє не палідроми.	