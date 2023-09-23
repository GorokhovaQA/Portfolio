Описание задач в рамках технического задания.
1. Задание по API: Напишите позитивные и негативные тест-кейсы на проверку ручки регистрации.

Есть запрос регистрации вида:

Request: api/v1/register

{ login: String, email: String; password: String; confirmPassword: String; }

Response:

{ code: int; result: String; }

Также есть ручка getUser, которая возвращает информацию о том, существует ли такой пользователь или нет. Необходимо проверить наличие пользователя.

Request: api/v1/getUser { login: String }

Response: { code: int; result: String; }

Все данные сохраняются в базу данных.

Дополнительный вопрос: как бы вы проверили работу данного функционала на сайте?

В результате выполнения задания мною были разработаны позитивные сценарии с валидными данными, а также негативные сценарии с валидными/невалидными данными (так как четких требований к заданию не прилагалось, мною, на основании опыта и здравого смысла, был составлен чек-лист с данными для позитивных и негативных проверок полей "Логин" и "Email") Для каждого тест-кейса были указаны тестовые данные, шаги и ожидаемый результат, а также были включены проверки статуса кода и структуры ответа.

Итоги: было разработано 11 тест-кейсов для проверки ручки регистрации.

2. Задание: Необходимо протестировать лифт в девятиэтажном доме.

Решение: В ходе выполнения задания был составлен чек-лист для тестирования лифта, выделены классы эквивалентности и предложены тестовые данные. Данный чек-лист включает функциональные проверки различных частей системы (лифта), тестирование безопасности, нагрузочное и стресс-тестирование, а также UX/UI проверки.

Итоги: было разработано 58 проверок для тестирования лифта.
