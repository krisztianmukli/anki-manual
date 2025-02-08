# Hiányzó könyvtárak

Ha az Anki nem indul el, kérlek, futtasd terminálból a `anki` parancsot. Ha azt mondja, hogy egy könyvtár hiányzik, telepítsd azt és próbáld újra.

Ha arra panaszkodik, hogy nincs elérhető platform, indítsd el az Anki-t a következő parancssorral, ami megmutatja, hogy ha hiányzik egy könyvtár:

```shell
QT_DEBUG_PLUGINS=1 anki
```

Miután telepítetted a könyvtárat az apt-get vagy hasonló segítségével, ismételd meg a folyamatot. Lehet, hogy ezt többször is meg kell tenned, mire az összes szükséges könyvtár települ.
