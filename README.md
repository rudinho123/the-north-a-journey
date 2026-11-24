# The North – A Journey

Slovenská statická webová aplikácia a PWA – historický sprievodca štyrmi dňami na severe Anglicka (26.–29. novembra 2026).

**Živá aplikácia:** https://rudinho123.github.io/the-north-a-journey/

## Obsah

- 26. 11. – Bradford a Leeds
- 27. 11. – Liverpool
- 28. 11. – Manchester
- 29. 11. – York a Yorkshire

Návratový deň 30. novembra nie je súčasťou sprievodcu.

## Lokálne spustenie

V koreňovom priečinku projektu spusti:

```bash
python3 -m http.server 8000
```

Potom otvor http://localhost:8000.

## Publikovanie

Projekt už používa GitHub Pages. Zmeny v hlavnej vetve `main` sa publikujú na vyššie uvedenej adrese. Nasadenie a zdrojové súbory sú v tomto repozitári.

## Denné sprístupňovanie

Kapitoly sa sprístupňujú podľa dátumu v časovom pásme `Europe/London` (26.–29. 11. 2026). Ide o jednoduchú klientsku kontrolu dátumu, nie o bezpečnostnú ochranu. Parameter `?preview=1` umožňuje náhľad kapitol pred ich sprístupnením.

## Fotografie a mapy

Fotografie sa načítavajú z Wikimedia Commons. Pri fotografiách sú uvedené autorské a licenčné informácie priamo v popisoch obrázkov. V kapitolách sú vložené mapy OpenStreetMap. Fotografie, vložené mapy a webové fonty vyžadujú internetové pripojenie.

## Offline režim

Service worker ukladá základné súbory aplikácie (HTML, CSS, JavaScript, manifest a ikony) do cache. Po prvom úspešnom načítaní tak môže byť dostupná základná štruktúra aplikácie a texty kapitol. Externé fotografie, mapy OpenStreetMap a webové fonty sa offline nemusia zobraziť.

## Úprava obsahu

- Texty, dátumy, trasy a fotografie: `app.js`
- Vzhľad a responzívne rozloženie: `styles.css`
- Základná štruktúra: `index.html`
- PWA cache: `sw.js`
- Inštalačné nastavenia: `manifest.webmanifest`
