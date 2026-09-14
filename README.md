# fil

## Commande `/aibi`

La commande `aibi` ouvre les réglages d'écran natifs pour préparer une
connexion filaire ou sans fil vers un iPad, une tablette Samsung ou un autre
appareil.

```sh
chmod 755 ./aibi
bash ./aibi wireless ipad
bash ./aibi wireless samsung
bash ./aibi wireless other
bash ./aibi wired ipad
bash ./aibi status
```

Pour utiliser exactement `/aibi` depuis n'importe quel dossier, installez-la
depuis le dossier du dépôt dans un répertoire présent dans le `PATH` :

```sh
sudo mkdir -p /usr/local/bin
sudo cp ./aibi /usr/local/bin/aibi
sudo chmod 755 /usr/local/bin/aibi
hash -r
aibi wireless ipad
```

Si `./aibi` renvoie `permission denied`, exécutez d'abord `chmod 755 ./aibi`
et utilisez `bash ./aibi ...`. Vérifiez aussi que `aibi` est bien le fichier
du dépôt (`file ./aibi` doit indiquer un script shell), et non un dossier ou
un fichier téléchargé depuis une page web.

Sur macOS, la commande ouvre Réglages Système > Écrans. Sur Linux, elle ouvre
le gestionnaire d'écrans GNOME, XFCE ou ARandR disponible. Pour un iPad, le
mode natif est Sidecar : dans Réglages Écrans, choisissez `Ajouter un écran`
et l'iPad. Une tablette Samsung n'est pas une destination native de second
écran sur macOS ; elle nécessite une application compatible.