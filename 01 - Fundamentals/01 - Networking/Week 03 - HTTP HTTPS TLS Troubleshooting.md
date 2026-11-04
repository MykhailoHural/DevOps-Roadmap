# Week 03 — HTTP, HTTPS, TLS & Troubleshooting

**Час:** 5–7 годин

## Теорія

- HTTP request / response.
- Methods, headers, status codes.
- HTTP/1.1, HTTP/2, HTTP/3 — концептуально.
- HTTPS та TLS handshake.
- Certificates, CA, hostname validation, expiration.
- Proxy vs reverse proxy.
- Load balancing — основи.

## Команди

```bash
curl -v https://example.com
curl -I https://example.com

openssl s_client   -connect example.com:443   -servername example.com   </dev/null

sudo ss -lntp
```

## Практика

- [[Labs/Lab 05 - Trace HTTP Request]]
- [[Labs/Lab 06 - Capture Network Traffic]]
- Усі сценарії з папки Troubleshooting.

## Контрольні питання

- Що відбувається після введення URL у браузері?
- Які етапи відбуваються до HTTP response?
- Що перевіряє TLS certificate validation?
- Чим proxy відрізняється від reverse proxy?
- Які причини 502 Bad Gateway?

## Результат тижня

Пояснюєш шлях запиту та вмієш локалізувати проблему між DNS, TCP, TLS і HTTP.
