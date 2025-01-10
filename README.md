# Spring Boot Security Demo

Этот проект представляет собой демонстрацию использования Spring Boot с настройками безопасности (Spring Security).

## Описание
Приложение реализует базовые CRUD-операции для управления пользователями и ролями, а также демонстрирует настройки безопасности:
- Авторизация и аутентификация с использованием Spring Security.
- Пользователи с ролью `ADMIN` имеют доступ к панели управления пользователями (`/admin`).
- Пользователи с ролью `USER` имеют доступ только к своей домашней странице (`/user`), где отображается их личная информация.
- Поддерживается назначение нескольких ролей для одного пользователя.
- Настроена страница логина и функция logout.

## Функциональность
1. **Роли и доступ:**
    - Администратор (`ADMIN`) может:
        - Управлять пользователями (CRUD).
        - Просматривать список пользователей.
    - Пользователь (`USER`) может:
        - Просматривать свои данные на странице `/user`.

2. **Функция logout:**
    - Доступна с любой страницы через кнопку "Logout".

3. **Настройка переходов после логина:**
    - Администратор направляется на страницу `/admin`.
    - Пользователь направляется на страницу `/user`.