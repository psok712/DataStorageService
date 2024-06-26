Необходимо разработать сервис для хранения информации о товарах.
(Сервис должен хранить данные о товарах в памяти)

## Сущности:

```
Товар
{
  Номер товара;
  Наименование товара;
  Цена товара;
  Вес товара;
  Вид товара{Общий, Бытовая химия, Техника, Продукты};
  Дата создания;
  Номер Склада;
}
```

## Задание

* Нужно реализовывать Grpc-сервис со следующими методами:
    * Создать товар
    * Получить список товаров с фильтрами (Дата создания, Вид товара, Склад) и пагинацией
    * Получить товар по Id
    * Обновить цену товара
* Реализовать Interceptor для логирования Request и Response;
* Реализовать Interceptor для обработки ошибок;
* Реализовать валидацию входящих запросов с помощью библиотеки FluentValidation
* При разработке не использовать никаких внешних источников данных (БД, редис и т.п.), данные должны храниться в оперативной памяти.

- Реализовать одновременно взаимодействие с приложением через http и grpc
- Методы создания и изменения сущности должны быть потокобезопасными


unit-tests
Необходимо:
1. Создать проект unit тестов (XUnit)
2. Написать unit тесты для методов Services (Используя Mock для связанных объектов)


integration-tests
1. Создать проект integration тестов (XUnit)
2. Написать интеграционные тесты на http ручки:
- Создать товар;
- Получить список товаров с фильтрами (Дата создания, Вид товара, Склад) и Пагинацией ();
- Получить товар по Id;
- Обновить цену товара;


Критерии выполнения задания:
1. Тестами покрыто большинство возможных позитивных и негативных сценариев
2. Все тесты должны проходить успешно
3. Код должен быть написан чисто, разделен на логические блоки.

## Задание на 10 баллов:

- Написать интеграционные тесты на grpc ручки

## Дедлайн

* Сдача 30 марта,, 23:59
* Проверка 2 апреля, 23:59



