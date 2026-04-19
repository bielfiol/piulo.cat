---
title: "Convertir imatge a PDF"
description: "Com podem convertir imatges a PDF?"
pubDate: "Sep 25 2024"
author: "Biel Fiol Garí"
heroImage: '../../assets/terminal.png'
---

Per convertir una imatge a PDF podem fer servir `convert` de les eines que podem trobar al paquet ImageMagick.

Si no el tenim instal·lat el podem instal·lar amb:

```bash
sudo apt install imagemagick
```

Després, per convertir la imatge a PDF basta amb fer servir `convert`.

```bash
convert imatge.jpg document.pdf
```

Si volem fer un PDF amb diverses imatges bastarà amb indicar les imatges i després el document final.

```bash
convert imatge1.jpg imatge2.jpg imatge3.jpg fitxer_amb_totes_les_imatges.pdf
```
