---
title: "Convertir un PDF a imatges"
description: "Com podem convertir un PDF a imatges?"
pubDate: "Feb 23 2022"
author: "Biel Fiol Garí"
heroImage: '../../assets/terminal.png'
---

Necessitava convertir un arxiu PDF a imatges. Cercant per la xarxa he trobat un exemple fent servir `pdftoppm`.

Des d’Ubuntu 20.04, sols he hagut d’executar la següent instrucció des d’un terminal:

```bash
pdftoppm -jpeg -r 300 input.pdf output
```

Ha exportat les diferents pàgines de l’arxiu `input.pdf` en diferents arxius JPEG amb el nom `output` que li he indicat seguit del comptador de pàgina. És a dir, `output-01.jpeg`, `output-02.jpeg`, …

Per conèixer les opcions que ens permet `pdftoppm` o bé feim servir el paràmetre `--help` o bé feim ús de `man pdftoppm`.
