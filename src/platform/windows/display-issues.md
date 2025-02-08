# Windows megjelenítési problémák

<!-- toc -->

A Windows rendszeren a képernyőtartalom háromféleképpen jeleníthető meg. Az alapértelmezett a _szoftveres_, ami lassabb, de a leginkább kompatibilis. Van két másik lehetőség, amely gyorsabb: _OpenGL_ és _ANGLE_. Ezek gyorsabbak, de előfordulhat, hogy nem működnek, vagy megjelenítési problémákat okozhatnak, például hiányzó menüsorokat, üres ablakokat stb. Hogy melyik működik jobban, az a számítógépedtől függ.

Ha megjelenítési problémákba ütközöl, megpróbálhatsz szoftveres módra váltani a parancssor segítségével:

```bat
echo software > %APPDATA%\Anki2\gldriver6
```

Vagy a PowerShell használatával:

```powershell
echo software > $env:APPDATA\Anki2\gldriver6
```

Ez nem fog semmit sem kiírni. Ezután újra elindíthatod az Ankit.

Az alapértelmezett viselkedés visszaállításához változtasd a `software`-t `auto`-ra, vagy töröld a fájlt.

Az Anki 23.10+ verzióban a grafikus vezérlőt a beállítások képernyőn is megváltoztathatod.

## Teljes képernyő

Az Anki 2.1.50+ teljes képernyős móddal érkezik, de különböző problémák miatt le kellett tiltani, ha `OpenGL` van használatban. A szoftveres renderelés bekapcsolása a fent leírtak szerint lehetővé teszi a teljes képernyős opció használatát, bár vedd figyelembe, hogy a renderelés teljesítménye csökkenhet.

Az Anki 23.10+ verzióban a teljes képernyős mód az alapértelmezett Direct3D illesztőprogrammal támogatott.
