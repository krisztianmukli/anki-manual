## Megjelenítési hibák Linuxon

A hardveres gyorsítás alapértelmezés szerint be van kapcsolva. Ha üres képernyőt vagy megjelenítési problémákat tapasztalsz, próbáld meg engedélyezni a szoftveres renderelést a terminál segítségével:

```
echo software > ~/.local/share/Anki2/gldriver6
```

Ha vissza szeretne váltani az alapértelmezettre, állítsa a `software` értéket `auto`-ra, vagy távolítsd el a fájlt.

Az Anki 23.10+ verzióban a grafikus vezérlőt a beállítások képernyőn is megváltoztathatod.
