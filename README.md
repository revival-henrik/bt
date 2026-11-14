# Börjes – prototyp

Statisk kopia av [borjes.se](https://borjes.se), sparad 2026-11-14, som utgångspunkt för en ny hemsida.

## Sidor

| Fil | Original |
|---|---|
| `index.html` | https://borjes.se/ |
| `kategori-vintertacken.html` | https://borjes.se/hast/hasttacken/vintertacken/ |
| `produkt.html` | https://borjes.se/vintertacke-freedom-turnout-300-g-p20225/ |
| `kundservice.html` | https://borjes.se/kundservice/ |
| `hitta-butik.html` | https://borjes.se/hitta-butik/ |

Bilder, typsnitt och CSS ligger under `assets/`. Länkar mellan de fem sidorna går lokalt; övriga länkar går till live-sajten.

## Visa lokalt

```sh
python3 -m http.server 8010   # 8000 används av kyrktorget
# öppna http://localhost:8010
```

## Att tänka på

- Sidorna är sparade *efter* att JavaScript har ritat upp dem, och alla skript (Vue, spårning, cookie-banner) är borttagna. Menyer, sliders, filter, varukorg och sök fungerar därför inte – det är en visuell prototyp.
- Ett fåtal bilder på startsidan laddas fortfarande från borjes.se.
