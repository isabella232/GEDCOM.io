---
title: GEDC
permalink: /terms/v7/GEDC.html
layout: none
redirect-from:
  - /terms/v7/GEDC
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/GEDC

standard tag: GEDC

descriptions:
  - GEDCOM
  - |
    A container for information about the entire document.
    
    It is recommended that applications write GEDC with its required subrecord
    VERS as the first substructure of HEAD.

payload: null

substructures:
  "https://gedcom.io/terms/v7/GEDC-VERS": "{1:1}"

superstructures:
  "HEAD pseudostructure": "{1:1}"
...

```
