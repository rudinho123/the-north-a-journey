# The North – A Journey

Slovenská statická PWA – štvordňový historický sprievodca severným Anglickom.

## Spustenie lokálne

V priečinku projektu spusti napríklad:

```bash
python3 -m http.server 8000
```

Potom otvor `http://localhost:8000`.

## Bezplatné publikovanie cez GitHub Pages

1. Vytvor nový **verejný** GitHub repository (keďže súkromie obsahu neriešime, je to najjednoduchšie riešenie).
2. Nahraj všetky súbory a priečinky z tohto projektu priamo do koreňového priečinka repository.
3. V `Settings → Pages` vyber `Deploy from a branch`, vetvu `main` a priečinok `/(root)`.
4. Po publikovaní GitHub zobrazí adresu webu. Túto jednu adresu môžeš poslať bratovi.

## Denné sprístupňovanie

Kapitoly sa sprístupňujú podľa lokálneho dátumu zariadenia: 26.–29. 11. 2026. Názvy budúcich kapitol sa dovtedy nezobrazujú. Texty nezverejňujú konkrétne miesta, ktoré by prezradili plánované zastávky; Liverpool je výnimkou, pretože história všetkých troch štadiónov je výslovne súčasťou zadania. Ide o jednoduchú klientsku kontrolu dátumu, nie o bezpečnostnú ochranu.

## Fotografie a licencie

Fotografie sa načítavajú z Wikimedia Commons. Pri každej fotografii je v aplikácii uvedený autor, licencia a odkaz na pôvodnú stránku súboru. Fotografie sa načítajú pri otvorení kapitoly; na ich zobrazenie je potrebné internetové pripojenie. Pri každej snímke je uvedený autor, licencia alebo stav verejnej domény a odkaz na pôvodný súbor. Pred ďalším použitím obrázkov si vždy skontroluj aktuálne podmienky na stránke Commons.

## Úprava obsahu

Texty, dátumy, titulky a fotografie jednotlivých dní sú v poli `chapters` v súbore `app.js`. Vzhľad upravuje `styles.css`.

## Offline režim

Aplikácia ukladá základné súbory rozhrania do cache. Samotné fotografie z Wikimedia Commons a prvé načítanie stránky vyžadujú internetové pripojenie.
