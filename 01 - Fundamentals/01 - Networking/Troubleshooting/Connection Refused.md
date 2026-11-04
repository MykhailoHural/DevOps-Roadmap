# Scenario — Connection Refused

## Симптом
Клієнт отримує connection refused.

## Діагностика

```bash
ss -lntp
nc -vz 127.0.0.1 8000
curl -v http://127.0.0.1:8000
```

## Завдання
- [ ] Перевірити listener.
- [ ] Перевірити правильність IP та port.
- [ ] Перевірити стан сервісу.
- [ ] Пояснити різницю між відсутнім listener та timeout.

## Incident report
- Symptoms:
- Hypothesis:
- Commands:
- Findings:
- Root cause:
- Resolution:
- Prevention:
