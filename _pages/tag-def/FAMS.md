---
title: FAMS
permalink: /terms/v7/FAMS.html
layout: none
redirect-from:
  - /terms/v7/FAMS
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/FAMS

standard tag: FAMS

descriptions:
  - Family spouse
  - The family in which an individual appears as a partner. See FAM for more.

payload: @<XREF:FAM>@

substructures:
  "https://gedcom.io/terms/v7/NOTE": "{0:M}"
  "https://gedcom.io/terms/v7/SNOTE": "{0:M}"

superstructures:
  "https://gedcom.io/terms/v7/record-INDI": "{0:M}"
...

```
