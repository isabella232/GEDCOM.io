---
title: ADR1
permalink: /terms/v7/ADR1.html
layout: none
redirect-from:
  - /terms/v7/ADR1
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/ADR1

standard tag: ADR1

descriptions:
  - Address Line 1
  - The first line of the address, used for indexing. This structure’s payload
    should be a single line of text equal to the first line of the
    corresponding ADDR. See ADDRESS_STRUCTURE for more.

payload: http://www.w3.org/2001/XMLSchema#string

substructures: []

superstructures:
  "https://gedcom.io/terms/v7/ADDR": "{0:1}"
...

```
