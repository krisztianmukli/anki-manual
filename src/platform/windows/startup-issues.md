# Windows indítási problémák

<!-- toc -->

## Nincs hiba, de az alkalmazás nem jelenik meg

Ha elindítod az Ankit, de az hibaüzenet nélkül, meg sem jelenik, akkor próbáld meg a következőket:

- Kapcsold le a külső kijelzőt, vagy ha van a többi kijelzőt.
- Telepítsd a [legfrissebb Anki verziót](https://apps.ankiweb.net/).
- Állítsd be a [tizedesjelzőt](https://forums.ankiweb.net/t/windows-update-broke-anki/1822/75), ha az nem pont.
- Teleptísd az Anki régi [2.1.35-alternate](https://github.com/ankitects/anki/releases/tag/2.1.35) verzióját.

## Windows frissítések

Az Anki indításakor a következő üzeneteket kaphatod:

- _Python DLL betöltési hiba_ (_Error loading Python DLL_)
- _A program nem tud elindulni, mert az api-ms-win.... hiányzik._ (_The program can't start because api-ms-win.... is missing_)
- _A runanki szkript indítása sikertelen_ (_Failed to execute script runanki_)
- _A pyi_rth_multiprocessing szkript végrehajtása sikertelen_ (_Failed to execute script pyi_rth_multiprocessing_)
- _A pyi_rth_win32comgenpy szkript végrehajtása sikertelen_ (_Failed to execute script pyi_rth_win32comgenpy_)

Ezek a hibák általában azért fordulnak elő, mert a számítógépen hiányzik egy Windows-frissítés vagy Windows-könyvtár.

Ilyenkor nyisd meg a Windows Update-t, és győződj meg róla, hogy minden frissítés telepítve van a gépedre. Ha bármit szükséges telepíteni, akkor indítsd újra a készüléket a telepítés után.

## Windows 7/8

Windows 7/8 rendszeren előfordulhat, hogy manuálisan kell telepítened a következő frissítéseket:

- <https://www.microsoft.com/en-us/download/details.aspx?id=48234>
- <https://aka.ms/vs/15/release/vc_redist.x64.exe>
- <http://www.catalog.update.microsoft.com/Search.aspx?q=kb4474419>
- <http://www.catalog.update.microsoft.com/Search.aspx?q=kb4490628>

## Videóillesztőprogram-problémák

Lásd a [megjelenítési problémák](./display-issues.md) oldalt.

## Több kijelző

Ha a _LoadLibrary failed with error 126_-os hibaüzenetet kapod, azt az okozhatja, hogy az Anki által használt eszközkészletnek gondjai vannak a [több kijelzővel](https://forums.ankiweb.net/t/error-126-on-open-anki-desktop/13967).

## Antivírus/tűzfal szoftver

A gépeden lévő harmadik féltől származó szoftverek megakadályozhatják az Anki betöltését. Megpróbálhatsz egy kivételt hozzáadni az Anki számára, vagy átmenetileg kikapcsolhatod a vírusirtót/tűzfalat, hátha ez segít.

## Adminisztrátori jogok

Egyes felhasználók arról számoltak be, hogy az Anki nem futatható, amíg nem kattintanak jobb gombbal az Anki ikonra, és nem választják a "Futtatás rendszergazdaként" lehetőséget. Az Anki minden adatát a felhasználói mappában tárolja, és nem igényel rendszergazdai jogosultságokat, de ezt is kipróbálhatod, ha már kimerítetted az összes többi lehetőséget.

## Frissítés után több Anki telepítés jelent meg

Ha a frissítési folyamat során több Anki-telepítés maradt (például a `C:\Program Files\Anki` és a `C:\Program Files (x86)\Anki` mappákban), előfordulhat, hogy ezek működőképtelen állapotban maradnak, és az Anki nem hajlandó elindulni hibaüzenetet nélkül.

Próbáld meg eltávolítani az Anki összes példányát a számítógépről. Ehhez keresd meg őket a Gépház > Alkalmazások és szolgáltatások (vagy Alkalmazások > Telepített alkalmazások) menüpontban, és távolítsd el őket, vagy futtasd az `uninstall.exe` programot az egyes Anki programmappákban. Ezt követően telepítsd újra az Ankit.

## Hibakeresés

Az Anki terminálból való indítása több információt adhat néhány hibáról. Miután telepítetted az Anki legújabb verzióját, és meggyőződtél róla, hogy az összes Windows-frissítés telepítve van, az Anki közvetlen futtatása helyett nyomd meg a <kbd>Windows</kbd> billentyűt (vagy nyisd meg a Start menüt), írd be a `cmd` parancsot, és indítsd el a parancssort. Amikor megnyílik a terminálablak, illesszd be a következő parancsot, majd nyomd le az <kbd>Enter</kbd>-t. (Az elérési útvonal más lesz, ha az Anki nem az alapértelmezett helyére van telepítve).

```
%LocalAppData%\Programs\Anki\anki-console.bat
```
Feltehetően az Anki ugyanúgy nem fog megnyílni, mint korábban, de a terminál ablakban megjelenő kimenet talán elárul valamit arról, hogy mi okozza a problémát.

## Ha semmi sem vezet eredményre

Ha a fenti megoldások kipróbálása után sem tudod elindítani az Ankit, két lehetőséged maradt:

- Próbáld meg [Python-ból indítani](https://faqs.ankiweb.net/running-from-python.html).
- Megpróbálhatsz egy régebbi Anki-verziót, amely egy régebbi eszközkészlettel készült, például a [2.1.35-alternate](https://github.com/ankitects/anki/releases/tag/2.1.35) vagy a [2.1.15](https://github.com/ankitects/anki/releases/tag/2.1.15)-öt.
