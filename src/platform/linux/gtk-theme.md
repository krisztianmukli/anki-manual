# Anki nem veszi fel a GTK témát Gnome/Linuxon

Ezt a problémát megkerülheti, ha kifejezetten megmondja az Ankinak, hogy melyik GTK témát használja. Futtasd a következő parancsokat egy terminálban:

```shell
theme=$(gsettings get org.gnome.desktop.interface gtk-theme)
echo "gtk-theme-name=$theme" >> ~/.gtkrc-2.0
echo "export GTK2_RC_FILES=$HOME/.gtkrc-2.0" >> ~/.profile
```

Ezután jelentkezz ki és vissza a számítógépedbe, az Anki fel fogja venni a GTK témát.
