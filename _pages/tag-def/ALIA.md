---
title: ALIA
permalink: /terms/v7/ALIA.html
layout: none
redirect-from:
  - /terms/v7/ALIA
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/ALIA

standard tag: ALIA

descriptions:
  - Alias
  - |
    A single individual may have facts distributed across multiple individual
    records, connected by ALIA pointers (named after “alias” in the computing
    sense, not the pseudonym sense).
    
    This specification does not define how to connect INDI records with ALIA.
    Some systems organize ALIA pointers to create a tree structure, with the
    root INDI record containing the composite view of all facts in the leaf
    INDI records. Others distribute events and attributes between INDI records
    mutually linked by symmetric pairs of ALIA pointers. A future version of
    this specification may adjust the definition of ALIA.

payload: @<XREF:INDI>@

substructures:
  "https://gedcom.io/terms/v7/PHRASE": "{0:1}"

superstructures:
  "https://gedcom.io/terms/v7/record-INDI": "{0:M}"
...

```
