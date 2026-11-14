# Börjes – PROTOTYP

> ⚠️ **Detta är en prototyp, inte Börjes riktiga webbshop.**
> Inga köp, inloggningar eller beställningar kan göras här.

Prototypen visas på **https://revival-henrik.github.io/bt/**

Repot innehåller en statisk kopia av Börjes webbshop, sparad 2026-11-14. Den används som utgångspunkt för design- och utvecklingsarbete med en ny hemsida.

Bilder, texter, produktinformation, logotyper och varumärken tillhör Börjes Tingsryd AB och respektive varumärkesägare. Priser och lagerstatus var aktuella när kopian sparades och kan ha ändrats sedan dess.

## Sidor

| Fil | Sida |
|---|---|
| `index.html` | Startsida |
| `kategori-vintertacken.html` | Kategori: Häst › Hästtäcken › Vintertäcken |
| `produkt.html` | Produkt: Vintertäcke Freedom Turnout 300 g |
| `kundservice.html` | Kundservice |
| `hitta-butik.html` | Hitta butik |

Bilder, typsnitt och CSS ligger under `assets/`.

## Märkning som prototyp

- Logotypen visar "Börjes PROTOTYP" med "DEMO" i fet röd text framför.
- Varje sida har en röd banner längst ner (alltid synlig) och "[PROTOTYP]" i fliktiteln.
- Det finns inga länkar till Börjes riktiga webbplatser. Länkar till de fem sidorna ovan går till prototypens sidor, och alla andra länkar går till prototypens startsida.
- Sidorna är märkta `noindex`, och `robots.txt` stänger ute sökmotorer.

## Visa lokalt

```sh
python3 -m http.server 8010   # 8000 används av kyrktorget
# öppna http://localhost:8010
```

## Publicering

GitHub Actions (`.github/workflows/pages.yml`) publicerar automatiskt till GitHub Pages vid varje push till `main`.

## Att tänka på

- Sidorna är sparade *efter* att JavaScript har ritat upp dem, och alla skript (Vue, spårning, cookie-banner) är borttagna. Menyer, sliders, filter, varukorg och sök fungerar därför inte – det är en visuell prototyp.
