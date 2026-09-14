# fil

## Commande `/aibi`

La commande `aibi` ouvre les réglages d'écran natifs pour préparer une
connexion filaire ou sans fil vers un appareil Apple, Samsung ou autre.

```sh
chmod +x aibi
./aibi wireless apple
./aibi wireless samsung
./aibi wireless other
./aibi wired apple
./aibi status
```

Pour utiliser exactement `/aibi` depuis n'importe quel dossier, installez-la
dans un répertoire présent dans le `PATH`, par exemple :

```sh
sudo install -m 755 aibi /usr/local/bin/aibi
```

Sur macOS, la commande ouvre Réglages Système > Écrans. Sur Linux, elle ouvre
le gestionnaire d'écrans GNOME, XFCE ou ARandR disponible. Le protocole sans
fil (AirPlay, Miracast, Chromecast ou Smart View) doit être pris en charge par
l'ordinateur et l'appareil cible.