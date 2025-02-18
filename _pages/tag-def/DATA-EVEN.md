---
title: DATA-EVEN
permalink: /terms/v7/DATA-EVEN.html
layout: none
redirect-from:
  - /terms/v7/DATA-EVEN
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/DATA-EVEN

standard tag: EVEN

descriptions:
  - Event
  - A list of enumerated values indicating the types of events that were
    recorded in a particular source. Each event type is separated by a comma
    and space. For example, a parish register of births, deaths, and marriages
    would be BIRT, DEAT, MARR.

payload: https://gedcom.io/terms/v7/type-List#Enum

enumeration values:
  ADOP: https://gedcom.io/terms/v7/ADOP
  ANUL: https://gedcom.io/terms/v7/ANUL
  BAPM: https://gedcom.io/terms/v7/BAPM
  BARM: https://gedcom.io/terms/v7/BARM
  BASM: https://gedcom.io/terms/v7/BASM
  BIRT: https://gedcom.io/terms/v7/BIRT
  BLES: https://gedcom.io/terms/v7/BLES
  BURI: https://gedcom.io/terms/v7/BURI
  CAST: https://gedcom.io/terms/v7/CAST
  CHR: https://gedcom.io/terms/v7/CHR
  CHRA: https://gedcom.io/terms/v7/CHRA
  CONF: https://gedcom.io/terms/v7/CONF
  CREM: https://gedcom.io/terms/v7/CREM
  DEAT: https://gedcom.io/terms/v7/DEAT
  DIV: https://gedcom.io/terms/v7/DIV
  DIVF: https://gedcom.io/terms/v7/DIVF
  DSCR: https://gedcom.io/terms/v7/DSCR
  EDUC: https://gedcom.io/terms/v7/EDUC
  EMIG: https://gedcom.io/terms/v7/EMIG
  ENGA: https://gedcom.io/terms/v7/ENGA
  CENS: https://gedcom.io/terms/v7/FAM-CENS
  NCHI: https://gedcom.io/terms/v7/FAM-NCHI
  RESI: https://gedcom.io/terms/v7/FAM-RESI
  FCOM: https://gedcom.io/terms/v7/FCOM
  GRAD: https://gedcom.io/terms/v7/GRAD
  IDNO: https://gedcom.io/terms/v7/IDNO
  IMMI: https://gedcom.io/terms/v7/IMMI
  CENS: https://gedcom.io/terms/v7/INDI-CENS
  NCHI: https://gedcom.io/terms/v7/INDI-NCHI
  RESI: https://gedcom.io/terms/v7/INDI-RESI
  MARB: https://gedcom.io/terms/v7/MARB
  MARC: https://gedcom.io/terms/v7/MARC
  MARL: https://gedcom.io/terms/v7/MARL
  MARR: https://gedcom.io/terms/v7/MARR
  MARS: https://gedcom.io/terms/v7/MARS
  NATI: https://gedcom.io/terms/v7/NATI
  NATU: https://gedcom.io/terms/v7/NATU
  NMR: https://gedcom.io/terms/v7/NMR
  OCCU: https://gedcom.io/terms/v7/OCCU
  ORDN: https://gedcom.io/terms/v7/ORDN
  PROB: https://gedcom.io/terms/v7/PROB
  PROP: https://gedcom.io/terms/v7/PROP
  RELI: https://gedcom.io/terms/v7/RELI
  RETI: https://gedcom.io/terms/v7/RETI
  SSN: https://gedcom.io/terms/v7/SSN
  TITL: https://gedcom.io/terms/v7/TITL
  WILL: https://gedcom.io/terms/v7/WILL

substructures:
  "https://gedcom.io/terms/v7/DATA-EVEN-DATE": "{0:1}"
  "https://gedcom.io/terms/v7/PLAC": "{0:1}"

superstructures:
  "https://gedcom.io/terms/v7/DATA": "{0:M}"
...

```
