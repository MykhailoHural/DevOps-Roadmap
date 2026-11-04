# Lab 06 — Capture Network Traffic

## Мета
Побачити TCP traffic локального HTTP service.

## Terminal 1

```bash
python3 -m http.server 8000 --bind 127.0.0.1
```

## Terminal 2

```bash
sudo tcpdump -ni lo 'tcp port 8000'
```

## Terminal 3

```bash
curl http://127.0.0.1:8000
```

Зупини capture через Ctrl+C.

## Завдання

- [ ] Знайти SYN.
- [ ] Знайти SYN-ACK.
- [ ] Знайти ACK.
- [ ] Знайти подальший обмін даними.
- [ ] Знайти завершення TCP connection, якщо воно потрапило у capture.

## Питання

- Що таке loopback interface?
- Чому використано `-i lo`?
- Що показує `-n`?
- Що означають SYN, SYN-ACK та ACK?

## Примітка

Це локальний навчальний traffic. Не запускай packet capture на чужих мережах або пристроях без дозволу.
