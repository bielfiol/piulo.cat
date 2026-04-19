---
title: "Reduir la mida d’un PDF (des de Linux)"
description: "Com poder reduir la mida d'un PDF?"
pubDate: "Dec 27 2023"
author: "Biel Fiol Garí"
heroImage: '../../assets/terminal.png'
---

Moltes vegades he de pujar arxius al registre digital d’administracions públiques i hi ha certes limitacions quant a la mida dels arxius (en el moment d’escriure l’entrada la limitació són 5 arxius que no poden excedir de 10 Mb i el total d’arxius no pot superar els 15 Mb).

```bash
gs -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dPDFSETTINGS=/ebook -dQUIET -dBATCH -sOutputFile=pdf_reduit.pdf pdf_original.pdf
```

Aquí teniu unes configuracions de `-dPDFSETTINGS`:

- `/screen` (72 dpi, mida petita i qualitat dolenta)
- `/ebook` (150 dpi, qualitat mitjana)
- `/printer` (300 dpi, qualitat alta)
- `/prepress` (300 dpi, qualitat alta preservant el color)
- `/default` (quasi idèntic a `screen`, però amb una qualitat lleugerament superior)
