# Notarize / Proof Connector — Connector Discovery

**Official Documentation:** https://notarize.com  
**Base URL:** https://api.notarize.com/v1  
**Auth Model:** API Key (Bearer Token)  

## Основные сущности вендора
- нотариальные транзакции (/transactions), документы, участники, верификационные свидетельства

## Лимиты и особенности API
- Соблюдение Rate Limits вендора, обработка HTTP 429 с экспоненциальным backoff.
- Валидация входных данных по Pydantic-схемам вендора до отправки запроса.
- Тестовая точка проверки подключения: `GET /v1/organizations/me`.
