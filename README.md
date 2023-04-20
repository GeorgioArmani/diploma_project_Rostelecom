###  Итоговый проект по автоматизированному тестированию функционала страницы https://b2c.passport.rt.ru сайта "Ростелеком"

#### При тестировании сайта были написаны:
- ручные чек-лист и тест-кейсы;
- баг-репорты;
- автоматизированные тесты (настроены на запуск через Run).

#### При тестировании сайта были применены следующие техники тест-дизайна:
- разбиение на классы эквивалентности;
- анализ граничных значений;
- тестирование состояний и переходов.

И в позитивных, и в негативных тестах для страницы восстановления пароля необходимо вручную вводить символы с картинки.

---------------------
#### Папка pages содержит следующие файлы:
- api_reg_email.py - GET-запросы к виртуальному почтовому ящику (1secmail.com) для получения валидного 
email и кода для регистрации на сайте и восстановления пароля;
- locators.py - локаторы XPath и CSS на web-элементы сайта;
- auth.py - функции-обёртки для локаторов, распределённые по классам в зависимости от тематики тестов   
- base.py - функции для применения к локаторам явных ожиданий, получения главной страницы сайта и пути текущей страницы   
- config.py - исходные статические данные   
- settings.py - учетные данные, используемые в процессе теста

#### Папка tests содержит следующие файлы: 
test_negative_auth_page - тестируем негативные сценарии страницы авторизации   
test_negative_reg_page - тестируем негативные сценарии страницы регистрации test_negative_new_pass_page - тестируем негативные сценарии страницы восстановления пароля   
test_positive_auth_page - тестируем позитивные сценарии страницы авторизации   
test_positive_reg_page - тестируем позитивные сценарии страницы регистрации   
test_positive_new_pass_page - тестируем позитивные сценарии страницы восстановления пароля
