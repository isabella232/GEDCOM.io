---
title: HEIGHT
permalink: /terms/v7/HEIGHT.html
layout: none
redirect-from:
  - /terms/v7/HEIGHT
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/HEIGHT

standard tag: HEIGHT

descriptions:
  - Height in pixels
  - |
    How many pixels to display vertically for the image. See CROP for more.
    
    HEIGHT is a number of pixels. The correct tag for the height of an
    individual is the DSCR attribute.
    
        0 @I45@ INDI
        1 DSCR brown eyes, 5ft 10in, 198 pounds

payload: http://www.w3.org/2001/XMLSchema#nonNegativeInteger

substructures: []

superstructures:
  "https://gedcom.io/terms/v7/CROP": "{0:1}"
...

```
