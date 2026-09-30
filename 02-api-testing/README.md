
# API-тестирование

Баг-репорт по POST-запросу через Postman.

## Что внутри

- [Баг-репорт API](./bug-report-api.md) — Yandex Cloud Functions

## Инструменты

- Postman v10
- Windows 11
- JSON

## Итог

Сервер возвращает 200 OK, но:
- переставляет поля (surname = отчество)
- меняет формат телефона
- не возвращает дату рождения
- принимает несуществующую дату 30.02.1999

Severity: Critical, Priority: High.
