---
title: NAME-TYPE
permalink: /terms/v7/NAME-TYPE.html
layout: none
redirect-from:
  - /terms/v7/NAME-TYPE
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/NAME-TYPE

standard tag: TYPE

descriptions:
  - Type
  - An enumerated value indicating the type of the name.

payload: https://gedcom.io/terms/v7/type-Enum

enumeration values:
  AKA: https://gedcom.io/terms/v7/enum-AKA
  BIRTH: https://gedcom.io/terms/v7/enum-BIRTH
  IMMIGRANT: https://gedcom.io/terms/v7/enum-IMMIGRANT
  MAIDEN: https://gedcom.io/terms/v7/enum-MAIDEN
  MARRIED: https://gedcom.io/terms/v7/enum-MARRIED
  OTHER: https://gedcom.io/terms/v7/enum-OTHER
  PROFESSIONAL: https://gedcom.io/terms/v7/enum-PROFESSIONAL

substructures:
  "https://gedcom.io/terms/v7/PHRASE": "{0:1}"

superstructures:
  "https://gedcom.io/terms/v7/INDI-NAME": "{0:1}"
...

```
