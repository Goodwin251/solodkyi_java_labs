﻿# [Лабораторна робота 2](https://github.com/Goodwin251/solodkyi_java_labs/blob/main/README.md)

Зробив Солодкий Ярослав ПД* 32

## Вимоги до функціоналу
Удосконалена система керування бібліотекою, має збергіати книги, DVD та зареєстрованих клієнтів. 

В тому числі вона має мати можливість:
1. Додавати предмети (книги, DVD) до бібліотеки.
1. Видаляти предмети з бібліотеки.
1. Реєструвати читача.
1. Видавати предмет читачеві.
1. Повертати предмет у бібліотеку.
1. Показувати список доступних предметів.
1. Показувати список взятих предметів та їхніх читачів

## Формат прийняття лабораторної роботи: 

1. Робота повинна мати план розробки програми та послідовність виконаних дій.
1. Код розробленого додатку прикріпити у вигляді посилання на GitHub.
1. GitHub повинен мати комміти як ви зробили на протязі розробки програми. Мова коммітів: Англійська.

## План розробки програми
1. Створити Maven проект в Eclipse.
1. Реалізувати абстрактний клас Item, інтерфейс IManageable.
1. Реалізувати класи Book, DVD, а також Patron.
1. Реалізувати клас Library, з використанням всіх створених класів в попередньому кроці.
1. Зробити приклад використання системи в класі App.
1. Створити репозиторій на GitHub.
1. Завантажити першу версію програми на репозиторій.
1. Зробити тестові класи TestBook, TestDVD, TestPatron, TestLibrary.

## Тести

### [Тести класу TestBook](https://github.com/Goodwin251/solodkyi_java_labs/blob/main/src/test/java/com/solodkyi/java_labs/Lab2Test/TestBook.java)
	*  testBookIsEqual *  перевірка порівняння однакових книг;
	*  testBookIsUnequal *  перевірка порівняння не однакових книг.

### [Тести класу TestDVD](https://github.com/Goodwin251/solodkyi_java_labs/blob/main/src/test/java/com/solodkyi/java_labs/Lab2Test/TestDVD.java)
	*  testDVDIsEqual *  перевірка порівняння однакових DVD;
	*  testDVDIsUnequal *  перевірка порівнняня не однакових DVD.
	*  testIncorrectDuration *  перевірка видання помилки у разі хибної тривалості DVD.

### [Тести класу TestPatron](https://github.com/Goodwin251/solodkyi_java_labs/blob/main/src/test/java/com/solodkyi/java_labs/Lab2Test/TestPatron.java)
	*  PatronIsEqual *  перевірка порівняння однакових клієнтів;
	*  PatronIsUnEqual *  перевірка порівняння не однакових клієнтів.

### [Тести класу TestLibrary](https://github.com/Goodwin251/solodkyi_java_labs/blob/main/src/test/java/com/solodkyi/java_labs/Lab2Test/TestLibrary.java)
	*  testAvaibleList *  перевірка правильності списку доступних предметів;
	*  testBorrowedList *  перевірка правильності списку заборгованих предметів;
	*  testAddItem *  перевірка додавання нових предметів у бібліотеку;
	*  testAddItemWithSameID *  перевірка додавання предмету з існуючим ідентифікатором;
	*  testAddBorrowedItem *  перевірка додвання запозиченого предмету;
	*  testRemoveItem *  первірка видалення передмету з бібліотеки;
	*  testRemoveNotExistedItem *  перевірка видалення не існуючого в бібліотеці предмету;
	*  testRegisterPatron *  перевірка регістрації клієнтів в бібліотекі;
	*  testRegisterPatronWithBorrowedItems *  перевірка регістрації клієнта з запозиченими предметами;
	*  testRegisterPatronWithSameID *  перевірка регістрації клієнта з існуючим ідентифікатором;
	*  testLendItem *  перевірка запозичення предмету бібліотеки зареєстрованим клієнтом;
	*  testLendBorrowedItem *  перевірка запозичення вже запозиченого предмету зареєстрованим клієнтом;
	*  testLendToUnRegistredPatron *  перевірка запозичення предмету бібліотеки незареєстрованим клієнтом;
	*  testLendUnRegisteredItem *  перевірка запозичення не існуючого в бібліотеці предмету зареєстрованим клієнтом;
	*  testReturnItem *  перевірка повернення предмету зареєстрованим клієнтом;
	*  testReturnAvaibleItem *  перевірка повернення вільного предмету зареєстрованим клієнтом;
	*  testReturnBorrowedItemFromWrongPatron *  перевірка повернення заборгованого предмету клієнтом, що не брав його.
