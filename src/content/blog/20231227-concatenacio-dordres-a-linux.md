---
title: "Concatenació d’ordres a Linux"
description: "Com concatenar ordres a Linux?"
pubDate: "Dec 27 2023"
author: "Biel Fiol Garí"
heroImage: '../../assets/terminal.png'
---

## Caràcter `|`

Amb el caràcter `|` podem fer que la sortida de la primera ordre es converteixi en entrada de la segona.

```bash
ordre1 | ordre2
```

Per exemple:

```bash
ls | more
dpkg --list | grep gnome
```

## Caràcter `&`

En aquest cas farà que les ordres s’executin alhora.

```bash
ordre1 & ordre2
```

També podem fer servir `&` per executar una ordre i que el procés s’executi mentre seguim treballant a la terminal.

```bash
ordre &
```

## Caràcters `||`

Amb `||` la segona ordre s’executarà si ha fallat la primera ordre.

```bash
ordre1 || ordre2
```

## Caràcters `&&`

La segona ordre sols s’executarà si la primera ordre acaba amb èxit.

```bash
ordre1 && ordre2
```

Exemple:

```bash
sudo apt update && sudo apt upgrade
```

## Caràcter `;`

Amb `;` la segona ordre s’executarà independentment que la primera ordre hagi tengut èxit o no.

```bash
ordre1 ; ordre2
```
