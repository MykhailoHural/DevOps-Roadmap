# Scenario — DNS Resolution Failure

## Симптом
Application не може звернутися до сервісу за доменним ім'ям. Пряме звернення до IP може працювати.

## Діагностика

```bash
getent hosts example.com
dig example.com
cat /etc/resolv.conf
```

## Завдання
- [ ] Перевірити, чи резолвиться домен.
- [ ] Перевірити resolver configuration.
- [ ] Відрізнити NXDOMAIN від timeout DNS query.
- [ ] Не робити висновок про доступність application лише з DNS lookup.

## Incident report
- Symptoms:
- Hypothesis:
- Commands:
- Findings:
- Root cause:
- Resolution:
- Prevention:
