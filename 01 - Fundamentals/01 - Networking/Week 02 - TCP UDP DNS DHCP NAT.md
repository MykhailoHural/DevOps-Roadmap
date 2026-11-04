# Week 02 — TCP, UDP, DNS, DHCP & NAT

**Час:** 5–7 годин

## Теорія

- TCP vs UDP.
- TCP three-way handshake.
- Ports та sockets.
- DNS resolver, recursive та authoritative DNS.
- Records: A, AAAA, CNAME, MX, TXT, NS.
- DHCP.
- NAT / PAT.
- Firewall fundamentals.
- Connection refused vs timeout.

## Команди

```bash
ss -tuln
sudo ss -tulpn
dig example.com
dig example.com A
dig example.com AAAA
dig example.com MX
dig @1.1.1.1 example.com
dig -x 1.1.1.1
```

## Практика

Виконай [[Labs/Lab 03 - Local TCP Server]] та [[Labs/Lab 04 - DNS Troubleshooting]].

## Контрольні питання

- Як працює TCP handshake?
- Чим TCP відрізняється від UDP?
- Що таке socket?
- Як працює DNS resolution?
- Що означає NXDOMAIN?
- Чому connection refused відрізняється від timeout?

## Результат тижня

Можеш створити локальний TCP service, перевірити його port та пояснити DNS lookup.
