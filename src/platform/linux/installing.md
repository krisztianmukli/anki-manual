# Anki telepítése és frissítése Linux alatt

<!-- toc -->

## Követelmények

A csomagolt verzióhoz egy friss 64 bites Intel/AMD Linux szükséges glibc-vel, valamint olyan közös könyvtárakkal, mint a libwayland-client és a systemd. Ha más architektúrán (pl. ARM/AArch64), vagy egy csupasz Linux disztribúción dolgozol, akkor lehetséges, hogy nem fogod tudni használni a csomagolt verziót, helyette próbáld meg [Python wheels](https://betas.ankiweb.net/#via-pypipip) csomagból telepíteni.

Debianon és származékain, mint például az Ubuntun és olyan [Chromebookokon ahol a Linux engedélyezve van](https://support.google.com/chromebook/answer/9145439?), használd a következőket telepítés előtt:

```shell
sudo apt install libxcb-xinerama0 libxcb-cursor0 libnss3
```

Ha az Anki nem indul el a telepítés után, akkor lehet, hogy [más könyvtárak hiányoznak](./missing-libraries.md).

Ha Ubuntu 24.04-et használsz, és az Anki nem indul el, nézd meg [ezt a témát](https://forums.ankiweb.net/t/issues-running-on-ubuntu-24-04/40974).

Az Anki build rendszere csak a glibc-t támogatja, így a musl-alapú disztribúciók jelenleg nem támogatottak.

## Telepítés

Az Anki telepítéséhez:

1. Töltsd le az Ankit a <https://apps.ankiweb.net> címről a Letöltések mappába.
2. Ha a zstd még nincs telepítve a rendszeredre, akkor telepítened kell (pl. `sudo apt install zstd`).
3. Nyiss egy terminált, és futtasd a következő parancsokat a megfelelő fájlnevek cseréjével.

```shell
tar xaf Downloads/anki-2XXX-linux-qt6.tar.zst
cd anki-2XXX-linux-qt6
sudo ./install.sh
```

Egyes Linux rendszereken szükség lehet a `tar xaf --use-compress-program=unzstd` használatára.

4. Ezután elindíthatod az Anki-t az 'anki' beírásával és az enter megnyomásával. Ha bármilyen problémával találkozol tekintsd meg a bal oldali linkeket.

## Frissítés

Ha korábban .deb/.rpm/etc-ről futtattad az Anki-t, kérlek, távolítsd el a rendszerverziót, mielőtt telepíted az itt található csomagot.

Ha egy korábbi csomagról frissítesz, egyszerűen ismételd meg a
a telepítés lépéseit a legújabb verzióra való frissítéshez. A felhasználói adatok megmaradnak.

Ha egy korábbi verzióhoz szeretnél visszatérni, kérjük, előbb mindenképpen végezd el a [visszaléptetést](http://changes.ankiweb.net).

## Kiegészítő kompatiblitás

Egyes kiegészítők nem mindig működnek a legújabb Anki-kiadással. Ha frissítesz a legújabb Anki verzióra, és úgy találod, hogy egy olyan kiegészítő, amely nélkül nem tudsz élni, nem működik, letöltheted a régebbi Anki verziókat a [kiadások oldalról](https://github.com/ankitects/anki/releases).

## Problémák

Ha az Anki telepítése vagy elindítása során bármilyen problémával találkozol, kérlek, tekintd meg a következő oldalakat:

- [Hiányzó könyvtárak](missing-libraries.md)
- [Megjelenítési hibák](display-issues.md)
- [Üres főablak](blank-window.md)
- [Linux disztró csomagok](distro-packages.md)
- [Hibás GTK téma](gtk-theme.md)
- [Wayland](wayland.md)
- [Beviteli módszerek](input-methods.md)
