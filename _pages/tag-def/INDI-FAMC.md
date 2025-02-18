---
title: INDI-FAMC
permalink: /terms/v7/INDI-FAMC.html
layout: none
redirect-from:
  - /terms/v7/INDI-FAMC
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/INDI-FAMC

standard tag: FAMC

descriptions:
  - Family child
  - The family in which an individual appears as a child. It is also used with
    a STAT substructure to show individuals who are not children of the family.
    See FAM and FAMC.STAT for more.

payload: @<XREF:FAM>@

substructures:
  "https://gedcom.io/terms/v7/FAMC-STAT": "{0:1}"
  "https://gedcom.io/terms/v7/NOTE": "{0:M}"
  "https://gedcom.io/terms/v7/PEDI": "{0:1}"
  "https://gedcom.io/terms/v7/SNOTE": "{0:M}"

superstructures:
  "https://gedcom.io/terms/v7/record-INDI": "{0:M}"
...

```
