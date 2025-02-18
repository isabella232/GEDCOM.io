---
title: PLAC-FORM
permalink: /terms/v7/PLAC-FORM.html
layout: none
redirect-from:
  - /terms/v7/PLAC-FORM
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/PLAC-FORM

standard tag: FORM

descriptions:
  - Format
  - |
    A comma-separated list of jurisdictional titles, which has the same number
    of elements and in the same order as the PLAC structure. As with PLAC, this
    shall be ordered from lowest to highest jurisdiction.
    
    The following represents Baltimore, a city that is not within a county.
    
        2 PLAC Baltimore, , Maryland, USA
        3 FORM City, County, State, Country

payload: https://gedcom.io/terms/v7/type-List#Text

substructures: []

superstructures:
  "https://gedcom.io/terms/v7/PLAC": "{0:1}"
...

```
