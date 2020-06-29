# PHP-Lab-3

Создаем базу данных и в ней таблицу  пользователей(users) с полями:
айдишник
логин
пароль
имя
фамилия
язык по умолчанию(поле может быть null)
роль(поле числовое, где клиент - 1, менеджер - 2,админ -3)
Перепиливаем авторизацию(вход на сайт) из предыдущей лабы, чтобы работало не из массива, а исходя из того есть ли пользователь в БД.

	Делаем страницы для базовых CRUD операций(создание, поиск, редактирование, удаление пользователей).
Страница список пользователей
	Страница где выводиться список пользователей(html таблицей). С выводом всех полей на экран кроме пароля. В каждой строке таблицы есть кнопки которые дают возможность удалить или отредактировать конкретного пользователя.При нажати на кнопку удлить, удаляем пользователя  и редиректим его обратно на эту же страницу, выводя сообщение о том то “пользователь такой-то успешно удален”.

Страница создания пользователя
Страница с полями ввода для всех колонок  таблицы кроме айдишника. При нажатии на кнопку “создать” формируеться insert запрос в базу данных который добавляет пользователя в таблицу users. После добавления в таблицу под пользователем можно авторизоваться на сайте.

Страница редактирования пользователя
Аналогично созданию, за исключением того что мы редактируем пользователя который уже есть, и при нажатии на кнопку “сохранить” мы изменяет в таблице уже существующего пользователя.

При желании страницы создания и редактирования можете делать в одном файле.

Страницы по редактированию и созданию доступны только админу. Страница со списком пользователей доступна только админу и менеджеру, но менеджер не может удалить, и не может перейти на страницу редактирования.
© 2020 GitHub, Inc.
