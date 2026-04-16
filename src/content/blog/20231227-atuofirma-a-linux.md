---
title: "AutoFirma a Linux"
description: "Què passa si amb autofirma no ens surten certificats?"
pubDate: 'Dec 27 2023'
author: "Biel Fiol Garí"
heroImage: '../../assets/blog-placeholder-1.jpg'
---

Per a signar digitalment documents faig servir AutoFirma del Portal Administración Electrónica (PAe).

## Descàrrega d'Autofirma

Es pot baixar el paquet d'AutoFirma per a la meva distribució (en el meu cas un paquet `.deb`) des de:

https://firmaelectronica.gob.es/Home/Descargas.html

## Problema amb certificats

Una vegada instal·lat vaig provar de signar un document però no em mostrava cap dels certificats instal·lats.
Tenia els certificats instal·lats al navegador Brave per a accerir a les pàgines d'administració pública.

Després de fer-hi moltes voltes vaig saber que AutoFirma, per defecte, va a cercar-los dins el magatzem del navegador Firefox.

## Solució

Com que no em funcionava accedir a AutoFirma des de Firefox i, com he dit, feia servir Brave, vaig provar:

👉 Obrir Firefox i afegir-hi els certificats.

Amb això AutoFirma ja detectava correctament els certificats.

## Nota

Segurament hi ha altres solucions, com fer servir directament el fitxer del certificat, però aquesta va funcionar correctament.