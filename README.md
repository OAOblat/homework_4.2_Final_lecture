## Тестирование возможности записаться на обучение профессии «Тестировщик ПО»

### 1. **Перечень автоматизируемых сценариев:**

* _Переход к форме записи на курс_

| Сценарий                                                     | Шаги воспроизведения                                                                                                                                                                                                                                                                                                                                                                                                           | Ожидаемый результат              |
|--------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|
| Через кнопку "Каталог курсов" в верхнем меню сайта           | 1. Перейти на главную страницу сайта https://netology.ru <br/>2. Нажать на кнопку "Каталог курсов" в верхнем меню сайта<br/>3. Нажать на кнопку "Программирование" в открывшемся меню "Направления обучения"<br/>4. Прокрутить список "Программирование" до профессии "Тестировщик ПО"<br/>5. Кликнуть по заголовку профессии "Тестировщик ПО"<br/>6. Кликнуть по кнопке "Записаться" на открывшейся странице                  | Открывается форма записи на курс |
| Через строку поиска по кнопке "Каталог курсов"               | 1. Перейти на главную страницу сайта https://netology.ru <br/>2. Нажать на кнопку "Каталог курсов" в верхнем меню сайта<br/>3. В строке поиска найти "Тестировщик ПО"<br/>4. Кликнуть по профессии "Тестировщик ПО"<br/>5. Кликнуть по кнопке "Записаться" в открывшейся странице профессии                                                                                                                                    | Открывается форма записи на курс |
| Через блок "Направления обучения" на главной странице сайта  | 1. Перейти на главную страницу сайта https://netology.ru <br/>2. Прокрутка до блока "Направления обучения"<br/>3. Кликнуть по блоку "Программирование"<br/>4. Прокрутить список "Программирование" до профессии "Тестировщик ПО"<br/>5. Кликнуть по заголовку профессии "Тестировщик ПО"<br/>6. Кликнуть по кнопке "Записаться" на открывшейся странице                                                                        | Открывается форма записи на курс |
| Через "Каталог курсов" в столбце "Обучение" в footer сайта   | 1. Перейти на главную страницу сайта https://netology.ru <br/>2. Прокрутка до футера сайта<br/>3. Кликнуть по "Каталог курсов" в столбце "Обучение"<br/>4. Нажать на кнопку "Программирование" в открывшемся меню "Все курсы"<br/>5. Прокрутить список "Программирование" до профессии "Тестировщик ПО"<br/>6. Кликнуть по заголовку профессии "Тестировщик ПО"<br/>7. Кликнуть по кнопке "Записаться" на открывшейся странице | Открывается форма записи на курс |
| Через "Программирование" в столбце "Обучение" в footer сайта | 1. Перейти на главную страницу сайта https://netology.ru <br/>2. Прокрутка до футера сайта<br/>3. Кликнуть по "Программирование" в столбце "Обучение"<br/>4. Прокрутить список "Программирование" до профессии "Тестировщик ПО"<br/>5. Кликнуть по заголовку профессии "Тестировщик ПО"<br/>6. Кликнуть по кнопке "Записаться" на открывшейся странице                                                                         | Открывается форма записи на курс |

**_Отправка формы "Записаться"_**

**Поле "Имя" должно соответствовать следующим требованиям:**
1. Обязательное поле: Пользователь должен обязательно заполнить это поле, чтобы отправить форму.
2. Длина имени: Имя должно быть не короче 2 символов и не длиннее 50 символов. Это ограничение помогает убедиться, что пользователь вводит адекватное и разумное значение для имени.
3. Разрешенные символы: 
- Использование кириллицы и латинницы
- Дополнительные символы: пробелы, дефисы (допустимы в середине)
- Запрет на специальные символы, таких как числа, знаки пунктуации или символы математических операций.
- Разрешенная буква Ё

**Поле "Телефон" должно соответствовать следующим требованиям:**
1. Содержит только арабские цифры
2. Знак "+" в начале
3. Количество цифр: 11

| Сценарий                                                                                                       | Шаги воспроизведения                                                                                                                                                  | Ожидаемый результат                                                                                   |
|----------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------|
| Отправка формы с валидными данными на кириллице(Проверка разрешенной буквы "Ё", девисов и пробелов в середине) | 1. В поле "Имя" ввести "Алёна"<br/>2. В поле "Телефон" ввести "+79990000000"<br/>3. Нажать кнопку "Записаться"                                                        | Появляется сообщение об успешной отправке заявки                                                      |
| Отправка формы с валидными данными на кириллице(Проверка дефиса в середине)                                    | 1. В поле "Имя" ввести "Анна-Мария"<br/>2. В поле "Телефон" ввести "+79990000000"<br/>3. Нажать кнопку "Записаться"                                                   | Появляется сообщение об успешной отправке заявки                                                      |
| Отправка формы с валидными данными на кириллице(Проверка пробела в середине)                                   | 1. В поле "Имя" ввести "Назим оглы"<br/>2. В поле "Телефон" ввести "+79990000000"<br/>3. Нажать кнопку "Записаться"                                                   | Появляется сообщение об успешной отправке заявки                                                      |
| Отправка формы с валидными данными на кириллице(Количество символов = 2)                                       | 1. В поле "Имя" ввести "Ян"<br/>2. В поле "Телефон" ввести "+79990000000"<br/>3. Нажать кнопку "Записаться"                                                           | Появляется сообщение об успешной отправке заявки                                                      |
| Отправка формы с валидными данными на кириллице(Количество символов = 50)                                      | 1. В поле "Имя" ввести "Александр Александр Александр Александр Александра"<br/>2. В поле "Телефон" ввести значение "+79990000000"<br/>3. Нажать кнопку "Записаться"  | Появляется сообщение об успешной отправке заявки                                                      |
| Отправка формы с валидными данными на латиннице                                                                | 1. В поле "Имя" ввести "Alex"<br/>2. В поле "Телефон" ввести "+79990000000"<br/>3. Нажать кнопку "Записаться"                                                         | Появляется сообщение об успешной отправке заявки                                                      |
| Отправка пустой формы                                                                                          | 1. Поле "Имя" оставить пустым<br/>2. Поле "Телефон" оставить пустым"<br/>3. Нажать кнопку "Записаться"                                                                | Появляются ошибки под каждым полем: "Обязательное поле". Заявка не отправлена                         |
| Отправка формы с пустым полем "Имя"                                                                            | 1. Оставить поле "Имя" пустым<br/>2. В поле "Телефон" ввести "+79990000000"<br/>3. Нажать кнопку "Записаться"                                                         | Появляется ошибка под полем "Имя": "Обязательное поле". Заявка не отправлена                          |
| Отправка формы с пустым полем "Телефон"                                                                        | 1. В поле "Имя" ввести значение "Алёна"<br/>2. Поле "Телефон" оставить пустым<br/>3. Нажать кнопку "Записаться"                                                       | Появляется ошибка под полем "Телефон": "Обязательное поле". Заявка не отправлена                      |
| Отправка формы с невалидными данными в поле "Имя" (Запрещенные символы)                                        | 1. В поле "Имя" ввести значение "25+?"<br/>2. В поле "Телефон" ввести значение "+79990000000"<br/>3. Нажать кнопку "Записаться"                                       | Появляется ошибка под полем "Имя": "Должно состоять из букв". Заявка не отправлена                    |
| Отправка формы с невалидными данными в поле "Имя" (Дефис в конце)                                              | 1. В поле "Имя" ввести значение "Иван-"<br/>2. В поле "Телефон" ввести значение "+79990000000"<br/>3. Нажать кнопку "Записаться"                                      | Появляется ошибка под полем "Имя": "Имя введено не верно". Заявка не отправлена                       |
| Отправка формы с невалидными данными в поле "Имя" (Дефис в начале)                                             | 1. В поле "Имя" ввести значение "-Иван"<br/>2. В поле "Телефон" ввести значение "+79990000000"<br/>3. Нажать кнопку "Записаться"                                      | Появляется ошибка под полем "Имя": "Имя введено не верно". Заявка не отправлена                       |
| Отправка формы с невалидными данными в поле "Имя" (Только пробелы)                                             | 1. В поле "Имя" ввести три раза пробел "  "<br/>2. В поле "Телефон" ввести значение "+79990000000"<br/>3. Нажать кнопку "Записаться"                                  | Появляется ошибка под полем "Имя": "Имя введено не верно". Заявка не отправлена                       |
| Отправка формы с невалидными данными в поле "Имя" (Количество символов 1)                                      | 1. В поле "Имя" ввести "Ф"<br/>2. В поле "Телефон" ввести значение "+79990000000"<br/>3. Нажать кнопку "Записаться"                                                   | Появляется ошибка под полем "Имя": "Имя введено не верно". Заявка не отправлена                       |
| Отправка формы с невалидными данными в поле "Имя" (Количество символов = 51)                                   | 1. В поле "Имя" ввести "Александра Александр Александр Александр Александра"<br/>2. В поле "Телефон" ввести значение "+79990000000"<br/>3. Нажать кнопку "Записаться" | Появляется ошибка под полем "Имя": "Превышено допустимое количество символов". Заявка не отправлена   |
| Отправка формы с невалидными данными в поле "Телефон" (Буквы вместо арабских цифр)                             | 1. В поле "Имя ввести значение "Алёна"<br/>2. В поле "Телефон" ввести значение"Алёна"<br/>3. Нажать кнопку "Записаться"                                               | Поялвяется ошибка под полем "Телефон": "Номер в формате +9 (999) 999-99-99". Заявка не отправлена     |
| Отправка формы с невалидными данными в поле "Телефон" (количество цифр меньше 11)                              | 1. В поле "Имя ввести значение "Алёна"<br/>2. В поле "Телефон" ввести значение"+7999000000"<br/>3. Нажать кнопку "Записаться"                                         | Поялвяется ошибка под полем "Телефон": "Номер в формате +9 (999) 999-99-99". Заявка не отправлена     |
| Отправка формы с невалидными данными в поле "Телефон" (нет знака "+" в начале)                                 | 1. В поле "Имя ввести значение "Алёна"<br/>2. В поле "Телефон" ввести значение"79990000000"<br/>3. Нажать кнопку "Записаться"                                         | Поялвяется ошибка под полем "Телефон": "Номер в формате +9 (999) 999-99-99". Заявка не отправлена     |



### 2. Перечень используемых инструментов с обоснованием выбора:

- _**Selenide**_: это инструмент автоматизации веб-приложений, он позволяет эмулировать действия пользователя в браузере, с ним работать проще чем с Selenium WebDriver, которая предлагает более простой и лаконичный способ написания автоматических тестов. Selenide использует только Java в качестве основного языка программирования, и т.к. тесты будем писать на Java, Selenide будет самым удобным вариантом.
- _**Java**_: язык программирования для написания автоматизированных тестов. Java является одним из наиболее популярных языков программирования для автоматизации тестирования.
- _**JUnit5**_: фреймворк для модульного тестирования Java-приложений, позволяет управлять ходом выполнения тестов и оценивать их результаты. Является более современной версией фреймворка для тестирования Java-приложений. Он предлагает множество преимуществ по сравнению с Junit4 и TestNG.
- _**Gradle**_: инструмент для автоматической сборки проектов на Java, более гибкая и мощная альтернатива Maven. Конфигурация проекта в Gradle намного более лаконична и компактна, чем в Maven.
- _**Git**_: для контроля версий и совместной работы над кодом
- _**IntelliJ IDEA**_: для разработки и отладки автоматизированных тестов
- _**Faker**_: для генерации случайных данных, библиотека упрощает работу по заполнению формы регистрации
- _**Rest Assured**_: для автотестирования REST API

При предоставлении доступа к базе данных для проверки успешной доставки заявки потребуется:
- _**DBeaver**_: для доступа к базе данных
- **Docker**_: для развертывания SUT и базы данных

### 3. Перечень необходимых разрешений, данных и доступов:

- Разрешение на автоматизацию процесса тестирования.
- Разрешение на заполнение формы записи на обучение
- Доступ к веб-сайту для выполнения автоматизированных сценариев.
- _Доступ к базе данных для проверки успешности отправки формы_ *

### 4. Перечень и описание возможных рисков при автоматизации:

- Изменение структуры или дизайна сайта может привести к необходимости пересмотра и корректировке тестовых сценариев.
- Изменение формы записи на обучение может привести к неработоспособности автоматизированных тестов. Для минимизации этого риска, необходимо регулярно проверять и обновлять автоматизированные тесты.
- Высокая стоимость разработки и поддержания тестов может превышать выгоду от их использования.

### 5. Перечень необходимых специалистов для автоматизации:

- Автоматизатор (тестировщик с навыками программирования): разрабатывает и поддерживает тесты.
    
### 6. Интервальная оценка с учётом рисков в часах:

- Оценка написания тест-плана: 3 часа
- Оценка написания автоматизированных тестов с использованием Selenide и Java: 6 часов
- Оценка регулярного обновления и поддержки автоматизированных тестов: 2 часа в месяц

Общая интервальная оценка с учетом рисков: 9-11 часов.