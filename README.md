# Mindset Vibecodera

Talk/prezentácia *Mindset Vibecodera* — Maroš Sollár.

Statická HTML prezentácia s per-slide audio narráciou. Audio sa pri prechode medzi slidmi spúšťa automaticky (prvý slide treba kliknutím ▶ odštartovať kvôli browser autoplay policy).

## Štruktúra

```
index.html        # celá prezentácia (HTML + CSS + JS)
audio/1.mp3 … 6.mp3   # narrácia pre každý slide
```

## Navigácia

- `→` / medzerník — ďalší slide
- `←` — späť
- `1` – `6` — skok na slide
- `?` — help

## Deploy

Live: <https://vibecoder.wanderhub.tech>

Server WANDERHUB, deploy cez rsync:

```bash
rsync -avz --delete index.html audio/ \
  root@wanderhub:/home/wanderhub-vibecoder/htdocs/vibecoder.wanderhub.tech/
```
