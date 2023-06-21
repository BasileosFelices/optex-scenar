# Scénář (screenplay) pro OpTeX
Semestrální práce pro BI-TEX
Filip Špelina 2023

Sada formátovacích maker pro snadnou sazbu divadelního scénáře.

## Stručné použití

Všechna potřebná makra se nachází v souboru `scenar.opm`. Tento soubor je třeba načíst s pomocí `\load[scenar]`.
Poté jsou k dispozici následující příkazy:

- `\beginscenar` nastaví automaticky doporučené formatovaní
- `\rep <nazev postavy> : <replika>` pro výpis formátované repliky 
    - `\pop {<text>}` pro popis děje, ktery se váže ke konkrétní replice
    - ! V případě použití \pop v rámci repliky je opravda třeba využít závorek {} 
- `\pop <text>` pro popis děje mimo repliku
- `\titlepage` vytiskne titulni stranu s danými parametry
    - `\title{<nazev>}` je jediný povinný parametr
    - `\subtitle{<nazev>}`
    - `\author{<text>}`
    - `\basedon{<text>}` pro specifikaci předlohy
    - `\date{<text>}`
- `\characterpage` vytiskne automaticky generovaný seznam postav
- `\contentpage` vytiskne obsah scén a dějství

V repozitáři je přiložená ukázka `pomada-example`.

## Dokumentace

Podrobnou dokumentaci v angličtině lze vygenerovat příkazem.

    optex -jobname scenar-doc '\docgen scenar'