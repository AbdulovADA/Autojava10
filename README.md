# План автоматизации тестирования формы "Запись на курс. Тестировщик ПО."

# Перечень автоматизируемых сценариев:

 ## Способы навигации к форме «Записаться на курс» по специальности Тестировщик ПО.

Способ 1:
1. На главной странице в верхней части выбрать пункт «Каталог курсов»
2. В левой части открывшегося окна навести курсор на направление «Программирование»
3. Во всплывшем списке, в подпункте «Для начинающих» выбрать направление «Тестировщик ПО»
4. В открывшемся окне выбрать пункт «Записаться»
5. В открывшемся окне появляется форма для заполнения контактных данных для записи на курсы или получения консультации.

Способ 2:
1. На главной странице, в блоках направлений обучения выбрать пункт «Программирование»
2. Скроллом вниз выбрать пункт «Тестировщик ПО»
3. В открывшемся окне выбрать пункт «Записаться»
4. В открывшемся окне появляется форма для заполнения контактных данных для записи на курсы или получения консультации.

Способ 3:
1. На главной странице сделать скролл вниз до футера странице.
2. В футере страницы в пункте «Обучение» выбрать «каталог курсов».
3. Скроллом вниз выбрать пункт «Тестировщик ПО»
4. В открывшемся окне выбрать пункт «Записаться»
5. В открывшемся окне появляется форма для заполнения контактных данных для записи на курсы или получения консультации.

Способ 4:
1. На главной странице сделать скролл вниз до футера странице.
2. В футере страницы в пункте «Обучение» выбрать «Популярные курсы».
3. Скроллом вниз выбрать пункт «Тестировщик ПО»
4. В открывшемся окне выбрать пункт «Записаться»
5. В открывшемся окне появляется форма для заполнения контактных данных для записи на курсы или получения консультации.

## Ui тестирование формы «Запись на курс»

1. (Незарегистрированный пользователь)
- Ввести валидные значения в поля Имя, Номер телефона, E-mail. 
- Нажать кнопку «Записаться». 
- Форма успешно отправлена. 
- СМС с подтверждением приходит на указанный телефон. Уведомление приходит на указанный e-mail.
2. (Зарегистрированный пользователь) 
- Ввести валидные значения в поля Имя, Номер телефона. 
- Нажать кнопку «Записаться». 
- Форма успешно отправлена. 
- СМС с подтверждением приходит на указанный телефон. 
3. Позитивное тестирование поля «Имя» (Зарегистрированный пользователь) 
- Ввести валидные значения в поле «Имя» 
- Ввести валидные значения в остальные поля 
- Нажать кнопку «Записаться» 
- Форма отправлена 
- СМС пришло на телефон, E-mail пришел на почту.
4. Позитивное тестирование поля «Номер телефона» (Зарегистрированные пользователь) -Ввести валидные значения в поле «Номер телефона» 
- Ввести валидные значения в остальные поля 
- Нажать кнопку «Записаться» 
- Форма отправлена 
- СМС пришло на телефон, E-mail пришел на почту. 
5. Позитивное тестирование поля «E-mail» (Незарегистрированные пользователь) 
- Ввести валидные значения в поле «E-mail» 
- Ввести валидные значения в остальные поля 
- Нажать кнопку «Записаться» 
- Форма отправлена 
- СМС пришло на телефон, E-mail пришел на почту. 
6. Негативное тестирование поля «Имя» (Зарегистрированный пользователь) 
- Ввести невалидные значения в поле «Имя» 
- Ввести валидные значения в остальные поля 
- Нажать кнопку «Записаться» 
- Форма отправлена 
- СМС пришло на телефон, E-mail пришел на почту.
7. Негативное тестирование поля «Номер телефона» (Зарегистрированные пользователь) 
- Ввести невалидные значения в поле «Номер телефона» 
- Ввести валидные значения в остальные поля 
- Нажать кнопку «Записаться» 
- Форма отправлена 
- СМС пришло на телефон, E-mail пришел на почту. 
8. Негативное тестирование поля «E-mail» (Незарегистрированные пользователь) 
- Ввести невалидные значения в поле «E-mail» 
- Ввести валидные значения в остальные поля 
- Нажать кнопку «Записаться» 
- Форма отправлена 
- СМС пришло на телефон, E-mail пришел на почту. 

# Перечень необходимых инструментов 

1. IntelliJ IDEA (Среда для автотестов)
2. Gradle. Система сборки кода
3. JUnit 5 Тестовая среда
4. Selenide Фреймворк для UI тестирования
5. REST Assured Фреймворк для API тестирования
6. Docker
7. Allure Система репортинга
8. SQL Система для написания запросов к БД
9. Faker Генерация данных 

# Перечень необходимых разрешений/данных/доступов

1. Разрешение на проведение тестирования сайта.
2. Доступ к БД / данным нескольких зарегистрированных пользователей необходимых для тестирования.

# Перечень и описание возможных рисков при автоматизации

1. Необходимость поддержки тестов в течение длительного времени.
2. Изменения в структуре и организации сайта, изменение верстки.

# Перечень необходимых специалистов для автоматизации

Необходим QA инженер по тестированию (навыки автотестов на Java)

# Интервальная оценка с учётом рисков (в часах)

На полный цикл, в который входят: написание тест-плана, предварительный сбор информации, подготовка тестового окружения, получение тестовых данных и доступа к ним, написание тестов, прогон тестов, выявление и устранение ошибок, повторный прогон тестов уходит от 40 до 80 часов.
