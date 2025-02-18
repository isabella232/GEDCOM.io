---
title: CREA
permalink: /terms/v7/CREA.html
layout: none
redirect-from:
  - /terms/v7/CREA
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/CREA

standard tag: CREA

descriptions:
  - Creation
  - The initial creation of the superstructure. This is metadata about the
    structure itself, not data about its subject. See CREATION_DATE for more.
  - The date of the initial creation of the superstructure. Because this refers
    to the initial creation, it should not be modified after the structure is
    created.

payload: null

substructures:
  "https://gedcom.io/terms/v7/DATE-exact": "{1:1}"

superstructures:
  "https://gedcom.io/terms/v7/record-FAM": "{0:1}"
  "https://gedcom.io/terms/v7/record-INDI": "{0:1}"
  "https://gedcom.io/terms/v7/record-OBJE": "{0:1}"
  "https://gedcom.io/terms/v7/record-REPO": "{0:1}"
  "https://gedcom.io/terms/v7/record-SNOTE": "{0:1}"
  "https://gedcom.io/terms/v7/record-SOUR": "{0:1}"
  "https://gedcom.io/terms/v7/record-SUBM": "{0:1}"
...

```
