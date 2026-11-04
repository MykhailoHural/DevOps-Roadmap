# Lab 04 — DNS Troubleshooting

## Команди

```bash
dig example.com
dig example.com A
dig example.com AAAA
dig @1.1.1.1 example.com
dig nonexistent-domain.invalid
```

## Завдання

- [ ] Знайти DNS server у відповіді.
- [ ] Порівняти A та AAAA.
- [ ] Порівняти запит до системного resolver та `1.1.1.1`.
- [ ] Знайти NXDOMAIN у відповіді для неіснуючого домену.
- [ ] Пояснити, чому DNS failure не тотожний TCP failure.

## Питання

1. Що таке recursive resolver?
2. Що означає NXDOMAIN?
3. Чи гарантує успішний DNS lookup доступність сервера?
4. Які наступні перевірки зробиш після успішного DNS lookup?
