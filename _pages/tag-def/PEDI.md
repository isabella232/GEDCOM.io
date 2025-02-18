---
title: PEDI
permalink: /terms/v7/PEDI.html
layout: none
redirect-from:
  - /terms/v7/PEDI
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/PEDI

standard tag: PEDI

descriptions:
  - Pedigree
  - An enumerated value indicating the type of child-to-family relationship
    represented by the superstructure.

payload: https://gedcom.io/terms/v7/type-Enum

enumeration values:
  ADOPTED: https://gedcom.io/terms/v7/enum-ADOPTED
  BIRTH: https://gedcom.io/terms/v7/enum-BIRTH
  FOSTER: https://gedcom.io/terms/v7/enum-FOSTER
  OTHER: https://gedcom.io/terms/v7/enum-OTHER
  SEALING: https://gedcom.io/terms/v7/enum-SEALING

substructures:
  "https://gedcom.io/terms/v7/PHRASE": "{0:1}"

superstructures:
  "https://gedcom.io/terms/v7/INDI-FAMC": "{0:1}"
...

```
