# Anki telepítése és frissítése macOS alatt

<!-- toc -->

## Követelmények

A macOS verziókövetelmények a letöltési oldalon találhatók.

Ha régi géped van, a régi verziót a [kiadások oldalról](https://github.com/ankitects/anki/releases) szerezheted be. A 24.11-es és korábbi Qt5 buildek támogatják a macOS 10.14-es és újabb verzióját. Ha a macOS 10.10 és 10.13 között vagy, akkor az [Anki 2.1.35-alternate](https://github.com/ankitects/anki/releases/tag/2.1.35) verziót kell használnod.

## Telepítés

1. Töltsd le az Ankit a <https://apps.ankiweb.net>-ről.
2. Mentsd el a fájlt az asztalra, vagy a Letöltések mappádba.
3. Nyisd meg és húzd az Anki-t az Alkalmazások mappádba vagy az asztalra.
4. Kattints duplán az Ankira abban a mappában ahova tetted.

## Frissítés

A frissítéshez zárd be az Ankit, ha nyitva van, majd kövesd a fenti lépéseket. Húzd az Anki ikonját ugyanarra a helyre, ahol korábban tároltad, és amikor erre felszólít, írd felül a régi verziót. A kártyák adatai megmaradnak.

## Homebrew

Ha [Homebrew](https://brew.sh/)-t használsz, telepítheted az Ankit a `brew install --cask anki` utasítás használatával a preferált Terminál alkalmazásban.

Frissítéshez használd a `brew upgrade`, eltávolításhoz a `brew uninstall --cask anki` parancsokat.

## Bővítmény kompatibilitás

Egyes kiegészítők nem mindig működnek a legújabb Anki-kiadással. Ha frissítesz a legújabb Anki verzióra, és úgy találod, hogy egy olyan kiegészítő, amely nélkül nem tudsz élni, nem működik, letöltheted a régebbi Anki verziókat a [kiadások oldalról](https://github.com/ankitects/anki/releases).

## Problémák

Ha az Anki telepítése vagy elindítása során bármilyen problémával találkozol, tekintsd meg a következőket:
- [Megjelenítési problémák](display-issues.md)
