---
title: FAMC-ADOP
permalink: /terms/v7/FAMC-ADOP.html
layout: none
redirect-from:
  - /terms/v7/FAMC-ADOP
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/FAMC-ADOP

standard tag: ADOP

descriptions:
  - Adoption
  - An enumerated value indicating which parent(s) in the family adopted this
    individual.

payload: https://gedcom.io/terms/v7/type-Enum

enumeration values:
  HUSB: https://gedcom.io/terms/v7/enum-ADOP-HUSB
  WIFE: https://gedcom.io/terms/v7/enum-ADOP-WIFE
  BOTH: https://gedcom.io/terms/v7/enum-BOTH

substructures:
  "https://gedcom.io/terms/v7/PHRASE": "{0:1}"

superstructures:
  "https://gedcom.io/terms/v7/ADOP-FAMC": "{0:1}"
...

```
