---
title: NO
permalink: /terms/v7/NO.html
layout: none
redirect-from:
  - /terms/v7/NO
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/NO

standard tag: NO

descriptions:
  - Did not happen
  - An enumerated value identifying an event type which did not occur to the
    superstructure’s subject. See NON_EVENT_STRUCTURE for more.
  - |
    Indicates that a specific type of event, given in the payload, did not
    happen within a given date period (or never happened if there is no DATE
    substructure).
    
    Substructures may provide discussion about the non-occurrence of the event
    but must not limit the meaning of what did not occur. No substructure other
    than DATE may restrict the breadth of that negative assertion.
    
    1 NO MARR means “no marriage occurred”
    
        1 NO MARR
        2 DATE TO 24 MAR 1880
    
    means “no marriage had occurred as of March 24^(th), 1880”

payload: https://gedcom.io/terms/v7/type-Enum

enumeration values:
  ADOP: https://gedcom.io/terms/v7/ADOP
  ANUL: https://gedcom.io/terms/v7/ANUL
  BAPM: https://gedcom.io/terms/v7/BAPM
  BARM: https://gedcom.io/terms/v7/BARM
  BASM: https://gedcom.io/terms/v7/BASM
  BIRT: https://gedcom.io/terms/v7/BIRT
  BLES: https://gedcom.io/terms/v7/BLES
  BURI: https://gedcom.io/terms/v7/BURI
  CHR: https://gedcom.io/terms/v7/CHR
  CHRA: https://gedcom.io/terms/v7/CHRA
  CONF: https://gedcom.io/terms/v7/CONF
  CREM: https://gedcom.io/terms/v7/CREM
  DEAT: https://gedcom.io/terms/v7/DEAT
  DIV: https://gedcom.io/terms/v7/DIV
  DIVF: https://gedcom.io/terms/v7/DIVF
  EMIG: https://gedcom.io/terms/v7/EMIG
  ENGA: https://gedcom.io/terms/v7/ENGA
  CENS: https://gedcom.io/terms/v7/FAM-CENS
  FCOM: https://gedcom.io/terms/v7/FCOM
  GRAD: https://gedcom.io/terms/v7/GRAD
  IMMI: https://gedcom.io/terms/v7/IMMI
  CENS: https://gedcom.io/terms/v7/INDI-CENS
  MARB: https://gedcom.io/terms/v7/MARB
  MARC: https://gedcom.io/terms/v7/MARC
  MARL: https://gedcom.io/terms/v7/MARL
  MARR: https://gedcom.io/terms/v7/MARR
  MARS: https://gedcom.io/terms/v7/MARS
  NATU: https://gedcom.io/terms/v7/NATU
  ORDN: https://gedcom.io/terms/v7/ORDN
  PROB: https://gedcom.io/terms/v7/PROB
  RETI: https://gedcom.io/terms/v7/RETI
  WILL: https://gedcom.io/terms/v7/WILL

substructures:
  "https://gedcom.io/terms/v7/NO-DATE": "{0:1}"
  "https://gedcom.io/terms/v7/NOTE": "{0:M}"
  "https://gedcom.io/terms/v7/SNOTE": "{0:M}"
  "https://gedcom.io/terms/v7/SOUR": "{0:M}"

superstructures:
  "https://gedcom.io/terms/v7/record-FAM": "{0:M}"
  "https://gedcom.io/terms/v7/record-INDI": "{0:M}"
...

```
