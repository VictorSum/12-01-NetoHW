# Домашнее задание к занятию 12.1 "Базы данных." - Виктор Сумской

Домашнее задание выполните в Google Docs и отправьте в личном кабинете на проверку ссылку на ваш документ.

Название файла должно содержать номер лекции и фамилию студента. Пример названия: "12.1 Базы данных - Александр Александров"

Перед тем как выслать ссылку, убедитесь, что ее содержимое не является приватным (открыто на просмотр всем, у кого есть ссылка). Если необходимо прикрепить дополнительные ссылки, просто добавьте их в свой Google Docs.

Любые вопросы по решению задач задавайте в чате учебной группы.

---
### Легенда

Заказчик передал Вам [файл в формате Excel](https://github.com/netology-code/sdb-homeworks/blob/main/resources/hw-12-1.xlsx), в котором сформирован отчет. 

На основе этого отчета, нужно выполнить следующие задания: 

### Задание 1.

Опишите таблицы (не менее 7), из которых состоит База данных:

- какие данные хранятся в этих таблицах,
- какой тип данных у столбцов в этих таблицах, если данные хранятся в PostgreSQL.

Приведите решение к следующему виду:

Сотрудники (

- идентификатор, первичный ключ, serial,
- фамилия varchar(50),
- ...
- идентификатор структурного подразделения, внешний ключ, integer).

Получилось 5 таблиц
Считаю нормализация таблиц (Адрес филиала, Тип подразделения) не имеет смысла там 3 записи. Накладные расходы при запросах будут больше чем просто каждый раз использовать запись (column value).

## Дополнительные задания (со звездочкой*)
Эти задания дополнительные (не обязательные к выполнению) и никак не повлияют на получение вами зачета по этому домашнему заданию. Вы можете их выполнить, если хотите глубже и/или шире разобраться в материале.  

https://github.com/VictorSum/12-01-NetoHW/blob/main/hw-12-1 .xlsx
### Задание 2*.

Перечислите, какие, на Ваш взгляд, в данной денормализованной таблице встречаются функциональные зависимости и какие правила вывода нужно применить, чтобы нормализовать данные. 

Зависимость между окладом и должности нет. Я не понимаю что за правила вывода применить? 
я  учел такую фичу как если человек работал на 2 проекта. Мне не нравится дата 31217. Для оклада можно использовать decimal/numeric
https://github.com/VictorSum/12-01-NetoHW/blob/main/hw-12-1 .xlsx 
