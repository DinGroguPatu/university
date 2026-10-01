# university

Saját készítésű egyetemi tanulóanyagok, GitHub Pages-en közzétéve.

**Élő oldal:** https://dingrogupatu.github.io/university/

## Tartalom

| Mappa | Tartalom |
|---|---|
| `iskolak-tanulokozossegek/` | Fogalomkártyák – Iskolák és tanuló közösségek (20 ZH-fogalom) |

## Felépítés

Minden anyag külön mappában lakik, és a mappa `index.html` fájlja a belépési pont,
így a gyökérben lévő `index.html` csak a mappákra hivatkozó nyitóoldal.
Új anyag hozzáadásához:

1. új mappa létrehozása (pl. `oktataselmelet/`),
2. az anyag feltöltése `index.html` néven a mappába,
3. link felvétele a gyökér `index.html` fájljának `.items` listájába.

Minden oldal egyetlen önálló HTML-fájl: nincs build-lépés, nincs függőség,
offline, fájlként megnyitva is működik.
