# Scénář (screenplay) pro OpTeX
Semestrální práce pro BI-TEX
Filip Špelina 2023

Sada formátovacích maker pro snadnou sazbu divadelního scénáře

## Použití

- `\load[scenar]` nacte tyto makra do vaseho dokumentu
- `\beginscenar` nastavi automaticky doporucene formatovani
- `\rep` \<nazev postavy\> : \<replika\> pro vypis repliky 
    - `\pop` {<text>} pro popis deje, ktery se vaze ke konkretni replice
- ``\pop`` \<text\> pro popis deje mimo repliku
- ``\titlepage`` vytiskne titulni stranu s danymi parametry
    - \title{\<nazev\>}
    - \subtitle{\<text\>}
    - \author{\<text\>}
    - \basedon{\<text\>}
    - \date{\<text\>}
- \characterpage vytiskne automaticky generovany seznam postav
- \contentpage vytiskne obsah scén a dějství

## Dokumentace

Podrobnou dokumentaci v angličitině lze vygenerovat příkazem.

    optex -jobname scenar-doc '\docgen scenar'