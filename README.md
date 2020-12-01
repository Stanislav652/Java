# Отчёт о тестировании приложения Main.java по переводу средств на банковский счет
Краткое описаниеен
05.12.2020 было проведено: тестирование приложения по переводу средств на банковский счет. Для тестирования использовали различные суммы банковского счета и  перевода денежных средств на счет.

Тестирование производилось в следующем окружении:

ОС: Windows 10 Home, 
64-разрядная Java: 11.0.9,
 IntelliJ IDEA 2020.2

На тестирование затрачено: 1,5 часа

##Описание тестов:
Тестирование проводилось путем подстановки различных значений в переменные account и transfer, чтобы увидеть, какие значения передаются в переменную total. Было использовано функциональное тестирование.

Для тестирования использовались тестовые данные из тестового сценария:

а) различные значения текущего состояния банковского счета, подстановка в переменную account

б) различные значения перевода денежных средств на счет, подстановка в переменную transfer

##Результаты
55% успешных / 45% неуспешных тестов


При проверке системы с большими значениями (account + transfer) выявлено следующее несоответствие: общая сумма (total) имеет отрицательное значение, т.к. используется тип данных int, который имеет границы  от -2 147 483 648 до 2 147 483 647.
