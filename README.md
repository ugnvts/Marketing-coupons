# Marketing coupons – prototipai

Barboros admin'o nuolaidos kodų ir programų perdarymo prototipai.

Vieša nuoroda: https://ugnvts.github.io/Marketing-coupons/

## Failai

| Failas | Kas tai | Nuoroda |
|---|---|---|
| `index.html` | Apvalkalas: ekranų ir variantų skirtukai | – |
| `puslapiai/kuponai.html` | Kuponų prototipas v1: Code groups, Codes and redemptions, Automatic programs; peržiūra, kūrimas, redagavimas | `#kuponai` |
| `scripts/build-pages.py` | Sugeneruoja `docs/` svetainę | – |
| `docs/` | GitHub Pages svetainė. **Ranka netaisyti** – generuojama skriptu | – |

## Kaip pridėti variantą

1. Naujas failas `puslapiai/<pavadinimas>.html`.
2. Eilutė `PAGES` sąraše faile `index.html`.

## Kaip atnaujinti svetainę

```bash
python3 scripts/build-pages.py
```

Tada commit ir GitHub Desktop'e **Push origin**.

## Kaip užšaldyti versiją

```bash
python3 scripts/build-pages.py --release "Kas šioje versijoje"
```

Užšaldyta versija (`docs/versijos/YYYY-MM-DD/`) niekada nesikeičia – tinka review ir patvirtinimams.

Saugykla vieša: čia nelaikyti konfidencialių failų (jiems – `archyvas/`, jis neįtraukiamas į git).
