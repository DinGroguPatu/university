# university

Saját készítésű egyetemi tanulóanyagok, GitHub Pages-en közzétéve.

**Élő oldal:** https://dingrogupatu.github.io/university/

## Tartalom

| Fájl / mappa | Tartalom |
|---|---|
| `index.html` | Nyitóoldal, innen nyílnak az anyagok |
| `theme.css` | **Közös színpaletta** – minden oldal innen veszi a színeit |
| `iskolak-tanulokozossegek/` | Fogalomkártyák – Iskolák és tanuló közösségek (20 ZH-fogalom) |

## Átszínezés

Minden szín a `theme.css` `:root` blokkjában van, CSS-változóként.
Egy érték átírása az egész oldalon érvényesül – a HTML-fájlokhoz nem kell hozzányúlni.
Jelenlegi paletta: sötétkék (`--navy`), zöld (`--green`), világosbarna (`--tan`), fehér alapon.

## Új anyag hozzáadása

1. Új mappa létrehozása (pl. `oktataselmelet/`), benne `index.html` néven az anyag.
2. A `<style>` blokk elé: `<link rel="stylesheet" href="../theme.css">`,
   és a fájlból törölhető a saját `:root { ... }` színblokk.
3. Egy `<a class="item">` blokk felvétele a gyökér `index.html` `.items` listájába.

Nincs build-lépés és nincs külső függőség; a `theme.css` az egyetlen közös fájl.
