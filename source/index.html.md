---
title: MicroF1 - API Docs

language_tabs:
  - php
  - json


toc_footers:

includes:
  - errors

search: true
---

# Пользователи 
## Добавить пользователя
### adduser


> **POST:**  https://api.com/v1/add/user

```php

```

```json

```

Данная команда используется при создании профиля клиента в системе.

Название | Значение | Описание
-------------- | -------------- | --------------
ИНН |	number 10 |	inn
ФИО |	text |	fio
Дата рождения |	calendar |	bdate
Вид паспорта |	drop-down list |	passport_view
Паспорт - серия |	Blank: text 2 |	passport_series_blank 
Паспорт - номер |	Blank: number 6 |	passport_number_blank
Паспорт - кем и когда выдан |	Blank: text + data |	passport_who_blank
Прописка |	text |	address_reg
Фактический адрес |	text |	address_fact
Телефон (мобильный) |	number 10 |	mobile_phone
Телефон (стационарный) |	number 10 |	home_phone
Компания |	text	| work_name
Телефон |	number 10 |	work_phone
Адрес (фактический) |	text |	work_address_fact
Адрес (юридический) |	text |	work_address_reg
Должность |	drop-down list |	work_post
Стаж (текущий)	| |	work_exp
Телефон |	number 10 |	contact_phone
Абонент |	text |	sub
Доход |	number 3-5 |	income
Другие источники - доход |	number 3-5 |	other_income
Другие источники - источник |	text |	other_source
Семейное положение |	drop-down list |	family_status
Дети |	drop-down list |	children


# Кредиты
## Создать заявку
### addcredit
Данная команда используется при создании новой кредитной заявки в системе.


> **POST:** https://api.com/v1/add/credit

```php

```

```json

```

Название | Значение | Описание
-------------- | -------------- | --------------
Сумма |	text |	amount
Срок |	text |	term
Процент |	text |	percent
Комментарий |	text |	comment
Номер карты банка | nubmer 16 | creditcard_number
Цель |	text |	purpose




## Получить статус
### creditstatus




> **GET:** https://api.com/api/v1/status/credit

```php

```

```json

```

Название | Значение | Описание
-------------- | -------------- | --------------
Номер кредита |	number | creditid




# Документы
## Получить договор
### creditdocs


> **GET:** https://api.com/api/v1/docs/credit

```php

```

```json

```

Название | Значение | Описание
-------------- | -------------- | --------------
Номер кредита |	number | creditid
ИНН |	number 10 |	inn
