# Scenario — TLS Certificate Error

## Можливі причини
- Certificate expired.
- Hostname mismatch.
- Incomplete certificate chain.
- Untrusted CA.
- Client/server time issue.

## Діагностика

```bash
openssl s_client   -connect example.com:443   -servername example.com   </dev/null
```

## Завдання
- [ ] Знайти subject та issuer.
- [ ] Перевірити validity dates.
- [ ] Перевірити hostname/SAN.
- [ ] Пояснити certificate chain.

## Incident report
- Symptoms:
- Hypothesis:
- Commands:
- Findings:
- Root cause:
- Resolution:
- Prevention:
