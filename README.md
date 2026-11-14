# Börjes – PROTOTYP

> ⚠️ **Detta är en prototyp, inte Börjes riktiga webbshop.**
> Inga köp, inloggningar eller beställningar kan göras här.
> Besök [borjes.se](https://borjes.se) för att handla.

Repot innehåller en statisk kopia av [borjes.se](https://borjes.se), sparad 2026-11-14. Den används som utgångspunkt för design- och utvecklingsarbete med en ny hemsida.

Bilder, texter, produktinformation, logotyper och varumärken tillhör Börjes Tingsryd AB och respektive varumärkesägare. Priser och lagerstatus var aktuella när kopian sparades och kan ha ändrats sedan dess.

## Sidor

| Fil | Original |
|---|---|
| `index.html` | https://borjes.se/ |
| `kategori-vintertacken.html` | https://borjes.se/hast/hasttacken/vintertacken/ |
| `produkt.html` | https://borjes.se/vintertacke-freedom-turnout-300-g-p20225/ |
| `kundservice.html` | https://borjes.se/kundservice/ |
| `hitta-butik.html` | https://borjes.se/hitta-butik/ |

Bilder, typsnitt och CSS ligger under `assets/`. Länkar mellan de fem sidorna går lokalt; övriga länkar går till live-sajten.

Logotypen visar "Börjes PROTOTYP", alla länkar till borjes.se pekar om till prototypen, och varje sida har en röd banner längst ner (alltid synlig) som visar att det är en prototyp. Sidorna är också märkta `noindex`, och `robots.txt` stänger ute sökmotorer.

## Visa lokalt

```sh
python3 -m http.server 8010   # 8000 används av kyrktorget
# öppna http://localhost:8010
```

## Att tänka på

- Sidorna är sparade *efter* att JavaScript har ritat upp dem, och alla skript (Vue, spårning, cookie-banner) är borttagna. Menyer, sliders, filter, varukorg och sök fungerar därför inte – det är en visuell prototyp.
- Ett fåtal bilder på startsidan laddas fortfarande från borjes.se.
