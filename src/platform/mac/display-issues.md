# macOS Megjelenítési problémák

<!-- toc -->

## Qt6 Videoillesztőprogram

Ha megjelenítési problémákat vagy összeomlást tapasztalsz az Anki 23.10+-ban, próbáld meg megváltoztatni a videóillesztő-programot a beállítások képernyőn, majd indítsd újra az Anki-t.

A régebbi Anki verziók nem adtak erre lehetőséget a beállításokban, de lehetővé tették az illesztőprogram beállítását a Terminal.app megnyitásával, majd a következő sor beillesztésével és az enter megnyomásával:

```
echo software > ~/Library/Application\ Support/Anki2/gldriver6
```

Ez nem fog semmit sem kiírni. Ezután újra kell indítanod az Ankit.

Ha vissza szeretne váltani az alapértelmezettre, állítsa a `software` értéket `auto`-ra, vagy távolítsd el a fájlt.

## Külső grafikus kártyák

Ha külső grafikus kártya használatával üres képernyőt tapasztalsz Mac-en, akkor a Ctrl nyomva tartása mellett kattints az Anki-ra, majd kattints a "Get Info" menüpontra és engedélyezd a "Prefer eGPU" opciót.

## Különböző felbontású monitorok

Nézd meg [ezt a fórum posztot](https://forums.ankiweb.net/t/mac-known-issues-wording-suggestion/7331).
