## Команда для запуска тестов:

### mvn test -Dtest="DemoQaTest"

## Задание:

1. Требуется автоматизировать 3 сценария.
2. Стек автоматизации:
    1. Java,
    2. Selenium/Selenide,
    3. jUnit5,
    4. Allure,
    5. Cucumber (по желанию)
3. Обязательно применение PageObject

## Формат сдачи работы:

- ссылка на репозиторий в git
- в файле `readme.md` должна быть описана команда для запуска тестов (maven или gradle). Запускать буду через командную
  строку

## Рекомендации:

1. Вы можете, по необходимости, ипользовать API сервиса https://demoqa.com/swagger/
    1. Подготовить предусловия
    2. Удалить данные после теста
    3. Создание пользовательской сессии
    4. и т.д.
2. Не забывайте про файл с конфигами. Не нужно хардкодить урды и настройки
3. Один класс – одна зона ответственности
4. Проследите, чтобы получился понятный отчет по тестированию

---------

### Предварительно выполнить руками 1 раз:

- Открыть страницу https://demoqa.com/register
- Создать себе аккаунт

### Сценарий 1:

1. Открыть страницу https://demoqa.com/login
3. Ввести логин и пароль
4. Перейти в раздел https://demoqa.com/profile
5. Проверить, что таблица пустая

### Сценарий 2:

1. Открыть страницу https://demoqa.com/login
3. Ввести логин и пароль
3. Перейти в раздел https://demoqa.com/books
4. Добавить в коллекцию 6 книг
5. Перейти в раздел https://demoqa.com/profile
6. Проверить, что в коллекции отображается 6 книг

### Сценарий 3:

1. Открыть страницу https://demoqa.com/login
3. Ввести логин и пароль
3. Перейти в раздел https://demoqa.com/books
4. Добавить в коллекцию 2 книги
5. Перейти в раздел https://demoqa.com/profile
6. Проверить, что в коллекции отображается 2 книги
7. Перейти в раздел https://demoqa.com/profile
8. Нажать Delete All Books
9. Вернуться в раздел https://demoqa.com/profile
10. Проверить, что таблица пустая