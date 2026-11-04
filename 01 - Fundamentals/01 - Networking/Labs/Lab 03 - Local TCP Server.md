# Lab 03 — Local TCP Server

## Мета
Побачити локальний TCP listener і різницю між успішним підключенням та connection refused.

## Підготовка

```bash
mkdir -p ~/networking-labs/week-02
cd ~/networking-labs/week-02
echo "Hello from local server" > index.html
```

## Terminal 1 — запусти сервер

```bash
python3 -m http.server 8000 --bind 127.0.0.1
```

## Terminal 2 — перевір

```bash
curl -v http://127.0.0.1:8000
ss -lntp
nc -vz 127.0.0.1 8000
```

## Зупини сервер через Ctrl+C і повтори перевірки

```bash
curl -v http://127.0.0.1:8000
nc -vz 127.0.0.1 8000
```

## Питання

- Який процес слухав порт?
- Яка адреса bind була задана?
- Чому після зупинки сервера connection не встановлюється?
- Що означає connection refused у цьому сценарії?

## Висновок
