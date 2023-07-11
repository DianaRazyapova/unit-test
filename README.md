# Unit Test

Этот репозиторий содержит набор юнит-тестов для тестирования части программы.

## Описание

Версия Java 11.

В проекте используется библиотека:

- JUnit 4
- Jacoco
- Mockito

## Запуск автотестов
Для запуска автотеста необходимо:

1. Склонируйте репозиторий на свой компьютер с помощью команды:

 ```sh
git clone git@github.com:DianaRazyapova/unit-test.git
```

2. Для создания отчета в Jacoco ввести команду

```sh   
mvn clean verify
```

## Структура проекта
```bash
pom.xml
README.md
.gitignore
src
|-- main
|   |-- java
|   |   |-- com
|   |   |   |-- example
|   |   |   |   |-- Animal.java
|   |   |   |   |-- Cat.java
|   |   |   |   |-- Feline.java
|   |   |   |   |-- Lion.java
|   |   |   |   |-- Predator.java
|-- test
|   |-- java
|   |   |-- CatMockTest.java
|   |   |-- FelineParametrizedTest.java
|   |   |-- FelineSpyTest.java
|   |   |-- LionMockTest.java
|   |   |-- LionParameterizedTest.java
```
## Выполненные задачи
1. Реализован принцип инъекции зависимостей для класса Lion, что позволило избежать его зависимости от класса Feline.
2. Написаны моки для зависимостей класса Lion с использованием Mockito.
3. Написаны тесты для классов Feline, Cat и Lion, включая параметризованные тесты, что позволило достичь высокого покрытия кода тестами не менее 100%.
4. Оценено покрытие кода тестами с помощью инструмента Jacoco, и достигнуто покрытие не менее 100% для классов Feline, Cat и Lion, что обеспечивает высокую надежность и качество кода.

## Отчет Jacoco
> Сгенерированные отчеты
<table>
     <tr>
        <td>
        <img width="1624" alt="Снимок экрана 2023-07-11 в 16 14 03" src="https://github.com/DianaRazyapova/unit-test/assets/115238502/fe4588cd-896a-4372-882a-228ee6ab708b">
        </td>
     </tr>
</table>
