---
title: ADR2
permalink: /terms/v7/ADR2.html
layout: none
redirect-from:
  - /terms/v7/ADR2
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/ADR2

standard tag: ADR2

descriptions:
  - Address Line 2
  - The second line of the address, used for indexing. This structure’s payload
    should be a single line of text equal to the second line of the
    corresponding ADDR. See ADDRESS_STRUCTURE for more.

payload: http://www.w3.org/2001/XMLSchema#string

substructures: []

superstructures:
  "https://gedcom.io/terms/v7/ADDR": "{0:1}"
...

```
