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

Projekt používa GitHub Pages. Zmeny v hlavnej vetve `main` sa publikujú na vyššie uvedenej adrese.

## Sprístupnenie kapitol

Všetky štyri dni a kapitoly sú dostupné ihneď; aplikácia ich nezamyká podľa dátumu.

## Fotografie, mapy a pripojenie

Fotografie sa načítavajú z Wikimedia Commons a ich popisy uvádzajú autorov a licencie. Úvodná schematická mapa Británie je súčasťou aplikácie. Fotografie a webové fonty vyžadujú internetové pripojenie.

## Offline režim

Service worker ukladá základné súbory aplikácie (HTML, CSS, JavaScript, manifest a ikony) do cache. Po prvom úspešnom načítaní môže byť dostupná základná štruktúra aplikácie a texty kapitol. Externé fotografie a webové fonty sa offline nemusia zobraziť.

## Úprava obsahu

- Texty, dátumy, trasy a fotografie: `app.js`
- Vzhľad a responzívne rozloženie: `styles.css`
- Základná štruktúra: `index.html`
- PWA cache: `sw.js`
- Inštalačné nastavenia: `manifest.webmanifest`
