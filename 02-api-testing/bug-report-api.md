# Баг-репорт: POST-запрос на Yandex Cloud Functions

**Severity:** Critical  
**Priority:** High  
**Тип:** Логический / API

---

## Окружение

- Postman v10
- Windows 11
- URL: https://functions.yandexcloud.net/d4e8qsrmeedndmefsus
- Метод: POST
- Content-Type: application/json

---

## Предусловие

Сервер доступен. В Postman настроен POST-запрос с заголовком Content-Type: application/json.

---

## Шаги воспроизведения

1. Открыть Postman.
2. Создать POST-запрос на указанный URL.
3. В теле запроса (raw JSON) отправить:

```json
{
  "birthday": "30.02.1999",
  "name": "Иван",
  "passport": "1234 567890",
  "patronymic": "Иванович",
  "phone": "89109991234",
  "surname": "Иванов"
}
