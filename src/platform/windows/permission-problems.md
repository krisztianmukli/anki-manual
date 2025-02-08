# Windows jogosultság problémák

<!-- toc -->

## Jogosultság problémák

Ha "hozzáférés megtagadva" üzeneteket kapsz, akkor az Anki néhány fájlja lehet, hogy csak olvasási módba van állítva, ami azt jelenti, hogy az Anki nem tudja írni őket.

A probléma javításához, tedd a következőket:

- a Start menü keresőmezőjébe írd be, hogy cmd.exe és üss egy Entert 
- a megnyíló ablakba írd be a következőt, és nyomd meg az Entert, hogy láthasd a felhasználóneved:

whoami

- írd be a következőket, minden sor után nyomd le az Entert, és a ____ helyett (a :F részt megtartva) írd be az előző parancstól megkapott felhasználónevet

cd %APPDATA%

icacls Anki2 /grant ____:F /t

Ez a parancs negjavítja az Anki adatmappájának jogosultságait, ezután elindíthatod a programot.

## Vírusírtó/Tűzfal/Anti-Malware

Néhány felhasználó "engedély megtagadva" vagy "csak olvasható" hibákat tapasztalt, amelyeket a gépükre telepített biztonsági szoftverek okoztak. Lehet, hogy kivételeket kell hozzáadnod az Anki számára, vagy megpróbálhatod ideiglenesen letiltani a szoftvert, hogy kizárd, hogy az okozza a problémát. Egyes felhasználók arról számoltak be, hogy a szoftver egyszerű kikapcsolása nem oldotta meg a problémát, és vagy hozzá kellett adniuk egy kivételt az Anki számára, vagy eltávolítaniuk a szoftvert.

## Jogosultsági problémák hibakeresése

Ha a problémák továbbra is fennállnak, miután kizártad a vírusirtót és a kapcsolódó programokat, végrehajtottad a fenti lépéseket az engedélyek javítására, és nem használod a OneDrive-ot, futtasd a következő parancsokat a cmd.exe programban, mindegyik után nyomd meg az Enter billentyűt.

whoami

cd %APPDATA%

icacls Anki2 /t

Ezután másold ki és illesszd be vagy készíts képernyőfotót arról, amit látsz, és küld el nekünk egy támogatási jegyben.
