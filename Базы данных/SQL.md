**SQL** - структурированный язык запросов, ориентированный на операции с данными, представленными в виде взаимосвязанных таблиц 
Язык определения данных **DDL** (Data Definition Language)
## Основные команды:
- CREATE TABLE
- ALTER TABLE
- FROP TABLE
- CREATE INDEX
- ALTER INDEX
- DROP INDEX
Язык манипулирования данными **DML** (Date Manipulation Language)
- INSERT
- UPDATE
- DELETE
Язык запросов **DQL** (Data Query Language)
- SELECT
У этой команды много опций и предложений, которые используются для формирования запросов к реляционной базе данных.
Язык управления данными **DCL** (Data Control Language) - контроль за выполняемыми действиями
- GRANT
- REVOKE
Команды управления транзакциями 
- COMMIT
- ROLLBACK
- SAVEPOINT
- SET TRANSACTION
## Типы данных
- integer
- smallint (до 5 значащих + знак)
- decimal (десятичное)
- float
- char(символьная строка до 255)
- var char (символьная строка переменной длины)
- date
- time
- datetime
- money
и т.д......
## Определения
> **Выражение** - комбинация операторов, констант, констант в явном представлении, функций, имён полей, элементов управления и свойств, в результате вычисления которых получается одно значение.

> **Инструкция (строка) SQL** - выражение, которое определяет команды на языке SQL.

> **Строковое выражение** - любое выражение, дающее непрерывную последовательность символов.

## Символы 
::= равно по определению
| - необходимость выбора одного из нескольких приведенных значений 
<...> - описанная с помощью метаязыка структура данных
{...} - обязательный выбор некоторой конструкции из списка
[...] - необязательный выбор некоторой конструкции из списка
[,...n] - необязательная возможность повторения конструкции от нуля до нескольких раз
## Идентификатор
- предназначены для обозначения объектов в базе данных и являются именами таблиц, представления, столбцов и других объектов базы данных
Используемые символы 
A-Z a-z 0-9 и __ пробелы низя
Ограничения на формат
- до 128 символов
- нет пробелов
- <>::=<буква>
- {<буква>|<цифра>}[,...n]
## Оператор SELECT
- SELECT [ALL|DISTINCT] {|[имя_столбца[AS новое_имя]]}[,...n]
- FROM имя_таблицы[[AS] псевдоним][,...n]
- [WHERE <условие_поиска>]
- [GROUP BY имя_столбца[,...n]]
- [HAVING <критерии выбора групп>]
- [ORDERED BY имя_столбца[,...n]]
## Последовательность выполнения
1. FROM - имена используемых таблиц
2. WHERE - фильтрация строк в соответствии с условиями
3. GROUP BY - образует группы строк, имеющих одно и то же значение в указанном столбце
4. HAVING - фильтруются группы строк объекта в соответствии с указанным условием
5. SELECT - какие столбцы должны присутствовать в выходных данных
6. ORDER BY - определяет упорядоченность результатов выполнения операторов
