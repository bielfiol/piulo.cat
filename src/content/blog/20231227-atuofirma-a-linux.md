---
title: "AutoFirma a Linux"
date: 2023-12-27
author: "Biel Fiol Garí"
---

Per a signar digitalment documents faig servir AutoFirma del Portal Administración Electrónica (PAe).

## Descàrrega

Es pot baixar el paquet d'AutoFirma per a la meva distribució (en el meu cas un paquet `.deb`) des de:

https://firmaelectronica.gob.es/Home/Descargas.html

## Problema amb certificats

Una vegada instal·lat vaig provar de signar un document però no em mostrava cap dels certificats instal·lats.

Després de fer-hi moltes voltes vaig saber que AutoFirma fa servir els certificats del navegador Firefox.

## Solució

Com que no em funcionava accedir a AutoFirma des de Firefox i feia servir Brave, vaig provar:

👉 Obrir Firefox i afegir-hi els certificats.

Amb això AutoFirma ja detectava correctament els certificats.

## Nota

Segurament hi ha altres solucions, però aquesta va funcionar correctament.