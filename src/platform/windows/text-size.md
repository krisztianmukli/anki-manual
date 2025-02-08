# Szövegméret

Ha úgy találod, hogy a szöveg nem megfelelő méretű, próbáld meg a következő környezeti változókat beállítani:

- Az ANKI_NOHIGHDPI=1 kikapcsolja a QT nagy DPI támogatásának egy részét

- Az ANKI_WEBSCALE=1 megváltoztatja az Anki webes nézeteinek (mint a pakli lista, a tanulóképernyő stb.) méretarányát, miközben a felület olyan elemeit, mint a menüsor, békén hagyja. Az 1-et helyettesítsd a kívánt méretaránnyal, például 1,5 vagy 0,75.

Windows alatt hozzáadhatod ezeket egy kötegelt parancsfájlhoz, hogy egyszerűsítsd az Anki indítását. Például hozz létre egy startanki.bat nevű fájlt az asztalodon, a következő tartalommal:

    set ANKI_WEBSCALE=0.75
    start "Anki" "C:\Program Files\Anki\anki"

Mentés után dupla kattintással indíthatod el az Anki-t a megadott beállításokkal.
