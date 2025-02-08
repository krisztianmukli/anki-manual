# Linux disztribúciók által terjesztett csomagok

Sok olyan problémát láttunk, amelyet az Anki Linux disztribúciók által terjesztett testreszabott verziói okoztak:

- Az Anki olyan harmadik féltől származó könyvtáraktól függ, mint a Qt, és a Linux disztribúciók gyakran helyettesítik e könyvtárak különböző verzióit anélkül, hogy tesztelnék a változások hatását.
- Előfordul, hogy az Anki általuk forgalmazott verziója több éves, vagy egy alfa/béta verzió, amelyet nem stabil kiadásra szántak. A disztribúciók gyakran kikapcsolják a beépített frissítés-ellenőrzést is, hogy ne kapjon értesítést az újabb verziókról.

Az Anki futtatható buildjei elérhetőek a <https://apps.ankiweb.net> oldalon. A legtöbb szükséges könyvtárat tartalmazzák, és az Anki tesztelve van, hogy ezekkel a könyvtárakkal működik. Ha problémákat tapasztalsz a disztribúciód verziójával, az első dolog, amit ki kell próbálnod, hogy átváltasz az általunk biztosított legújabb csomagolt verzióra.

Nyugodtan használhatod továbbra is a disztribúciód Anki verzióját, ha szeretnéd, de ha bármilyen problémába ütközöl, azt a disztribúciód csomagkarbantartóinak kell jelentened.
