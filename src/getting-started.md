# Kezdő lépések

<!-- toc -->

## Telepítés és frissítés

Kérjük, tekintsd meg a számítógépedhez tartozó utasításokat:

- [Windows](./platform/windows/installing.md)
- [Mac](./platform/mac/installing.md)
- [Linux](./platform/linux/installing.md)

## Videók

Ha gyorsan szeretnél elmerülni az Ankiban, nézd meg ezeket a bemutatkozó videókat. Némelyik egy korábbi Anki verzióval készült, de a koncepció ugyanaz.

- [Megosztott paklik és a felülvizsgálat alapjai](http://www.youtube.com/watch?v=QS2G-k2hQyg&yt:cc=on)

- [Szinkronizálás](https://www.youtube.com/watch?v=YkiM4DPzSVc&list=PLGgmaKOIHykFoomqkBJAyGiDQ2kyiuTao&yt:cc=on)

- [Kártyák sorrendjének megváltoztatása](http://www.youtube.com/watch?v=DnbKwHEQ1mA&yt:cc=on)

- [Kártyák formázása](http://www.youtube.com/watch?v=F1j1Zx0mXME&yt:cc=on)

- [Válasz beírása](http://www.youtube.com/watch?v=5tYObQ3ocrw&yt:cc=on)

Ha a YouTube nem érhető el az országodban, akkor a [töltsd le a videókat](https://apps.ankiweb.net/downloads/archive/screencasts/2.0/) helyette.

## Kulcsfogalmak

### Kártyák

A kérdés-válasz párost _kártyának_ nevezzük. Ez olyan, mint egy papír tanulókártya, amelynek az elején a kérdés, a hátoldalán pedig a válasz található. Az Ankiban azonban a kártya nem úgy néz ki, mint egy fizikai kártya, és amikor megmutatja a választ, a kérdés alapértelmezés szerint látható marad. Ha például alapfokú kémiát tanulsz, akkor egy olyan kérdést láthatsz, mint pl:

    K: Mi az oxigén kémiai szimbóluma?

Miután eldöntötte, hogy a válasz O, kattintson a "Válasz megjelenítése" gombra, és az Anki megmutatja:

    K: Mi az oxigén kémiai szimbóluma?
    V: O

A helyes válasz megerősítése után add meg az Ankinak, hogy mennyire jól emlékszel a válaszra, és az Anki eldönti, hogy mikor mutassa meg újra a kártyát. Anki például dönthet úgy, hogy 3 nap múlva újra megmutatja a kártyát. Ebben az esetben azt mondjuk, hogy a kártyának most 3 napos intervalluma van.

#### Kártya állapotok

<div id="types-of-cards" />

- **Új:** Kártyák, amelyeket letöltöttél vagy saját magad készítettél, de még soha nem tanulmányoztad őket.

- **Tanulás:** Kártyák, amelyeket a közelmúltban láttál először, és amelyeket még mindig tanulsz.

- **Felülvizsgálat:** Kártyák, amelyek tanulása befejeződött. Ezek a kártyák a késleltetésük (intervallum) letelte után ismét megjelennek.
  Kétféle felülvizsgálat állapotú kártya létezik:
  - **Friss:** A friss kártya olyan kártya, amelynek az időintervalluma 21 napnál rövidebb.
  - **Veterán:** A veterán kártya olyan kártya, amelynek az időintervalluma 21 nap vagy annál hosszabb.

- **Újratanulás:** Kártyák, amelyeket az átnézési szakaszban elfelejtettél. Ezek a kártyák visszakerülnek az újratanulási állapotba, hogy újra megtanuld őket.

### Paklik

A _pakli_ kártyák csoportja. A kártyákat különböző paklikba helyezheted, hogy a kártyagyűjteményed egyes részeit tanulmányozhasd, ahelyett, hogy mindent egyszerre tanulmányoznál. Minden paklihoz különböző beállítások tartozhatnak, például, hogy naponta hány új kártyát mutasson meg, vagy hogy mennyi ideig várjon a kártyák újbóli megjelenítéséig.

A paklik tartalmazhatnak más paklikat, ami lehetővé teszi, hogy a paklikat egy fába rendezd. Az Anki kettős kettőspontokat ("::") használ a paklifán belüli különböző szintek jelölésére. Például a "Kínai::Hanzi" nevű pakli a "Hanzi" paklira utal, amely a "Kínai" pakli része. Ha a "Hanzi" lehetőséget választod, akkor csak a Hanzi kártyák jelennek meg; ha a "Kínai" lehetőséget választod, akkor az összes kínai kártya megjelenik, beleértve a Hanzi kártyákat is.

A paklikat a fán belül úgy helyezheted el, hogy vagy elnevezed őket, és az egyes szintek között dupla kettőspontot teszel, vagy pedig a paklik listáján belül húzod őket. A másik paklikon belül elhelyezett paklikat gyakran "alpakliknak", a legfelső szintű paklikat pedig "szülőpakliknak" nevezik.

Az Anki egy "Alapértelmezett" nevű paklival indul; minden olyan kártya, amely valahogyan elkülönült a többi pakliból, ide kerül. Az Anki elrejti az alapértelmezett paklit, ha az nem tartalmaz kártyákat, és más paklikat is felvettél. Alternatívaként átnevezheted ezt a paklit, és használhatod más kártyák számára.

A paklik a paklilistában ábécé sorrendben vannak. Ez meglepő sorrendet eredményezhet, ha a paklik nevei számokat tartalmaznak. Például a "Pakli 10" a "Pakli 9" elé kerül, mivel az 1 a 9 előtt van. Ha azt szeretnéd, hogy a "Pakli 9" előbb jelenjen meg, átnevezheted "Pakli 09"-re, amely a "Pakli 10" előtt jelenik meg.

A kártyapaklikat a legjobb a kártyák széles kategóriáinak, nem pedig az olyan konkrét témáknak a tárolására használni, mint például az "ételek" vagy az "1. lecke". Erről bővebb információt a [paklik megfelelő használatáról](editing.md#using-decks-appropriately) szóló részben találsz.

Arról, hogy a paklik sorrendje hogyan befolyásolja a kártyák tanulmányozásának sorrendjét, lásd a [megjelenítési sorrendre](studying.md#display-order) vonatkozó részt.

### Jegyzetek és mezők

A tanulókártyák készítésekor gyakran javasolt, hogy egynél több kártyát készítsünk, amelyek ugyanarra az információra vonatkoznak. Ha például franciát tanulsz, és megtudod, hogy a bonjour szó azt jelenti, hogy "helló", akkor érdemes egy olyan kártyát készítened, amelyen a "bonjour" szó szerepel, és arra kérdez rá, mennyire emlékszel a "helló" szóra, és egy másik kártyát, amelyen a "helló" szó szerepel, és arra kérdez rá, mennyire jegyezted meg a "bonjour" szót. Az egyik kártya a francia szó felismerésének képességét teszteli, a másik kártya pedig a szó aktív felidézését méri.

Ha papír tanulókártyákat használsz, ebben az esetben az egyetlen lehetőség, hogy kétszer írod ki az információt, egyszer minden kártyára. Egyes tanulókártya-programok megkönnyítik az életet azzal, hogy az elülső és a hátsó oldal megfordítására szolgáló funkciót biztosítanak. Ez előrelépés a papíralapú helyzethez képest, de két nagy hátránya van:

- Mivel az ilyen programok nem követik külön a felismerési és az aktív felidézési teljesítményedet, a kártyákat általában nem az optimális időben mutatják meg neked, ami azt jelenti, hogy többet felejtesz el, mint szeretnél, vagy többet tanulsz, mint szükséges lenne.

- A kérdés és a válasz megfordítása csak akkor működik, ha mindkét oldalon pontosan ugyanazt a tartalmat szeretnéd. Ez azt jelenti, hogy például nem lehetséges extra információkat megjeleníteni a kártyák hátoldalán.

Az Anki megoldja ezeket a problémákat azzal, hogy lehetővé teszi a kártyák tartalmának különálló információkra való felosztását. Ezután megmondhatod az Ankinak, hogy melyik információ melyik kártyán szerepeljen, és az Anki gondoskodik a kártyák elkészítéséről, és frissíti azokat, ha a jövőben bármilyen módosítást végzel.

Képzeljük el, hogy francia szókincset akarunk tanulni, és minden kártya hátoldalán szerepeltetni akarunk egy tankönyvi oldalszámot. Azt szeretnénk, ha a kártyáink így néznének ki:

    K: Bonjour
    V: Helló
       12. oldal

És így:

    K: Helló
    V: Bonjour
       12. oldal

Mindkét kártyán ugyanaz a három kapcsolódó információ található: egy francia szó, egy angol jelentés és egy oldalszám. Ha összerakjuk őket, így néznek ki:

    Francia: Bonjour
    Magyar: Helló
    Oldal: 12

Az Ankiben a kapcsolódó információknak ezt a gyűjteményét _jegyzetnek_ nevezzük, és minden egyes információ egy _mezőben_ található. Ebben a példában a jegyzetnek három mezője van: "Francia", "Angol" és "Oldal".

A mezők hozzáadásához és szerkesztéséhez kattints a "Mezők..." gombra a jegyzetek hozzáadása vagy szerkesztése közben. A mezőkkel kapcsolatos további információkért lásd a [Mezők testreszabása](editing.md#customizing-fields) című részt.

### Kártyatípusok

Ahhoz, hogy az Anki képes legyen kártyákat készíteni a jegyzeteink alapján, meg kell adnunk neki egy tervezetet, amely megmondja, hogy mely mezők jelenjenek meg az egyes kártyák elülső vagy hátsó oldalán. Ezt a tervezetet _kártyatípusnak_ nevezzük. Minden jegyzettípushoz egy vagy több kártyatípus tartozhat; amikor jegyzetet adunk hozzá, az Anki minden kártyatípushoz létrehoz egy-egy kártyát.

Minden kártyatípusnak két sablonja van, egy a kérdéshez és egy a válaszhoz. Az előző francia példában azt akartuk, hogy a felismerő kártyánk hátoldala így nézzen ki:

    K: Bonjour
    V: Helló
       12. oldal

Ehhez beállíthatjuk a válasz sablonját::

    K: {{French}}
    V: {{English}}<br>
       {{Page}}. oldal

A kártyasablonokban a mezőnevek dupla szögletes zárójelbe vannak zárva, mint például {{French}} vagy {{English}}. Az Anki ezeket a mezőkben található tényleges szöveggel helyettesíti. Ezt nevezzük a ["mező cseréjének"](templates/fields.md). A nem dupla szögletes zárójelbe tett szöveg minden kártyán ugyanúgy jelenik meg. Például nem kell minden jegyzethez hozzáadnunk az ". oldal" szöveget, mert a sablon automatikusan hozzáadja minden kártyához. A `<br>` tag egy speciális kód, amely azt mondja az Ankinak, hogy lépjen a következő sorra. A részletekért lásd a [sablonok](templates/intro.md) részben.

Az aktív felimserést tesztelő kártya sablonjai is hasonló módon működnek majd.:

    K: {{English}}
    V: {{French}}<br>
       {{Page}}. oldal

Miután létrehoztunk egy kártyatípust, minden alkalommal, amikor új jegyzetet adunk hozzá, az adott kártyatípuson alapuló kártya jön létre. A kártyatípusok megkönnyítik a kártyák egységes formázását, és jelentősen csökkenthetik az információk hozzáadásával járó erőfeszítéseket. Azt is jelentik, hogy az Anki biztosítani tudja, hogy a kapcsolódó kártyák ne jelenjenek meg túl közel egymáshoz, és lehetővé teszik, hogy egyszer javítson ki egy gépelési hibát vagy ténybeli tévedést, és az összes kapcsolódó kártya egyszerre frissüljön.

A kártyatípusok hozzáadásához és szerkesztéséhez kattints a "Kártyák..." gombra a jegyzetek hozzáadása vagy szerkesztése közben. A kártyatípusokról további információkat a [Kártyák és sablonok](templates/intro.md) részben találhatsz.

### Jegyzettípusok

Az Anki lehetővé teszi, hogy különböző típusú jegyzeteket hozzon létre különböző anyagokhoz. Minden jegyzettípusnak saját mezői és kártyatípusai vannak. Jó ötlet, ha minden egyes tágabb témakörhöz, amelyet tanulmányoz, külön jegyzettípust hoz létre. Az előző francia példában egy "Francia" nevű jegyzettípust hozhatnánk létre ehhez. Ha fővárosokat szeretnénk tanulni, akkor ehhez is létrehozhatnánk egy jegyzettípust, olyan mezőkkel, mint az "Ország" és a "Főváros".

Az Anki néhány standard jegyzettípust tartalmaz. Ezek a jegyzettípusok azért vannak megadva, hogy megkönnyítsék az Anki használatát az új felhasználók számára, de hosszú távon ajánlott saját jegyzettípusokat létrehozni, kifejezetten a tanult tartalomhoz. A standard jegyzettípusok a következők:

- **Alap**\
  "Előlap" és "Hátlap" mezőkkel rendelkezik, és egy kártyát hoz létre. Az "Előlap" mezőbe beírt szöveg a kártya előlapján, a "Hátlap" mezőbe beírt szöveg pedig a kártya hátoldalán jelenik meg.

- **Alap (mindkét irányban)**\
  Mint az "Alap", de két kártyát hoz létre a beírt szöveghez: eleje→hátulja és hátulja→eleje.

- **Alap (egyik vagy mindkét irányban)**\
  Olyan, mint az "Alap", de van egy harmadik mezője, az "Ellenkező irány hozzáadása". Ha bármilyen szöveget írsz ebbe a mezőbe, akkor egy fordított (hátul→elöl) kártya is létrejön. A részleteket lásd a [Kártyák és sablonok](templates/intro.md) szakaszban.

- **Alap (írja be a választ)**\
  Ez lényegében az "Alap", egy extra szövegdobozzal az elején, ahová beírhatod a választ. Amikor a hátlapot feltárja, az Anki megmutatja a beírt és a tényleges válasz közötti különbségeket. A részletekért lásd a [Válaszod ellenőrzése](templates/fields.md#checking-your-answer) című részt.

- **Lyukas szöveg**\
  Egy jegyzettípus, lehetővé teszi a szöveg kijelölését és elrejtését (pl. "Az emberek [...] landoltak a Holdon." → "Az emberek 1969-ben landoltak a Holdon"). A részleteket lásd a [Lyukas szöveg](editing.md#cloze-deletion) szakaszban.

- **Képkitakarás**\
  Olyan, mint a "Lyukas szöveg" jegyzettípus, de szöveg helyett képekkel dolgozik, ami különösen akkor hasznos, ha olyan anyagot tanulsz, amely nagymértékben támaszkodik a képekre, például anatómia és földrajz. A részleteket lásd a kézikönyv [Képkitakarás](editing.md#image-occlusion) című részében.

Saját jegyzettípusok hozzáadásához és a meglévők módosításához az Anki főablakában az Eszközök → Jegyzettípusok kezelése menüpontot használhatod.

A jegyzetek és a jegyzettípusok az egész gyűjteményben közösek, nem korlátozódnak egy-egy paklira. Ez azt jelenti, hogy különböző jegyzettípusokat használhatsz egyetlen pakliban, vagy az ugyanabból a jegyzetből generált kártyákat különböző paklikba helyezheted. Amikor jegyzeteket adsz hozzá a Hozzáadás ablak segítségével, kiválaszthatod, hogy milyen jegyzettípust és milyen paklit használjon, és ezek a választások egymástól teljesen függetlenek.
A [jegyzetek típusát megváltoztathatod](browsing.md#notes) a jegyzetek létrehozása után is.

### Gyűjtemény

A _gyűjteményed_ az Ankiben tárolt összes anyagod: a kártyáid, jegyzeteid, paklijaid, jegyzettípusaid, pakli beállításaid, és így tovább.

## Megosztott paklik

A [Megosztott paklikról és a felülvizsgálat alapjairól](http://www.youtube.com/watch?v=QS2G-k2hQyg&yt:cc=on) szóló videót a YouTube-on nézheted meg.

A legegyszerűbb módja az Anki használatának, ha letöltesz egy pakli kártyát, amelyet valaki más osztott meg:

1. Kattints a "Megosztott tartalmak" gombra a pakli lista alján.

2. Ha megtaláltad a számodra érdekes paklit, kattints a "Letöltés" gombra, és töltsd le a paklicsomagot.

3. Kattints duplán a letöltött csomagra, hogy importáld azt az Anki-ba, vagy válassza a Fájl → Importálás menüpontot.

Megjegyzés: Jelenleg nem lehetséges megosztott paklikat közvetlenül az AnkiWeb fiókjához hozzáadni. Először importálnod kell őket az asztali alkalmazásba, az AnkiMobile-ba vagy az AnkiDroidba, majd [szinkronizálni](./syncing.md) kell őket, hogy feltöltsd a paklikat az AnkiWebre.

Egy komplex téma elsajátításának leghatékonyabb módja a saját pakli elkészítése. Az olyan tantárgyakat, mint a nyelvek és a tudományok, nem lehet egyszerűen a tények bemagolásával megérteni - magyarázatra és összefüggésekre van szükség a hatékony tanuláshoz. Ráadásul az információk saját magad általi bevitele arra kényszerít, hogy eldöntsd, melyek a kulcspontok, ami jobb megértéshez vezet.

Ha Ön nyelvtanuló, akkor talán kísértésbe esik, hogy letöltsön egy hosszú listát a szavakról és fordításukról, de ez ugyanúgy nem tanít meg egy nyelvet, mint ahogy a tudományos egyenletek memorizálása sem tanít meg asztrofizikára. A megfelelő tanuláshoz szükséged lehet tankönyvekre, tanárokra vagy valós mondatokkal való találkozásra.

    Ne tanulj, ha nem érted.
    --SuperMemo

A legtöbb megosztott paklit olyan emberek hozzák létre, akik az Ankin kívülről tanulják az anyagot, például tankönyvekből, órákról, tévéből stb. Kiválasztják az érdekes pontokat abból, amit tanulnak, és beteszik az Anki-ba. Lehet, hogy nem tesznek erőfeszítést arra, hogy háttérinformációkat vagy magyarázatokat adjanak a kártyákhoz, mert már értik az anyagot. Így amikor valaki más letölti a paklijukat, és megpróbálja használni, nagyon nehéz dolga lehet, mivel hiányoznak a háttérinformációk és a magyarázatok.

Ez nem jelenti azt, hogy a megosztott paklik használhatatlanok. Ha egy adott tananyagból tanulsz, és valaki megosztott egy paklit a tananyagban szereplő fogalmakkal, az egy nagyszerű módja annak, hogy időt takaríts meg. Egyszerű témák esetén, amelyek lényegében tények listájából állnak – például fővárosok nevei vagy országzászlók –, valószínűleg nincs szükséged külső forrásokra. Összetettebb témák esetén azonban a megosztott paklikat _kiegészítésként_ kell használni, nem pedig a külső tananyagok _helyettesítésére_.
