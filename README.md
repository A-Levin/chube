# chube
Charity Cube. A web application for charity organizations to manage their donations and volunteers.

There are three modules:
1. chube-core: the main module for donations and projects.
2. chube-bot: the module for administrators.
3. chube-volunteer: the module for volunteers.
Stack:
    Telegram Бот (Python):
        Библиотека: python-telegram-bot
        Фронт-энд: Mini Apps или Apps.

    API для Бота (Python):
        Фреймворк: FastAPI (асинхронный, поддержка OpenAPI).
        Валидация данных: Pydantic.
        Платежи: Интеграция с Stripe API.

    База данных:
        Реляционная БД: PostgreSQL.

    Логирование:
        Стек ELK: Elasticsearch, Logstash, Kibana.

    Системы управления контейнерами:
        Docker и Docker Compose.

    Безопасность:
        Протокол HTTPS.
        OAuth2 для авторизации и аутентификации.

    Тестирование:
        Pytest для тестирования.
        Factory Boy для создания тестовых данных.

Структура проекта:
backend - Основное приложение, API
bot - Телеграм бот, связывающий фронт и бэк
frontend - Фронтенд, miniapps by tg, react
