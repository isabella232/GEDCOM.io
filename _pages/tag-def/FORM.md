---
title: FORM
permalink: /terms/v7/FORM.html
layout: none
redirect-from:
  - /terms/v7/FORM
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/FORM

standard tag: FORM

descriptions:
  - Format
  - The media type of the file referenced by the superstructure. This should be
    a valid media type as defined by BCP 13. A registry of media types is
    maintained publicly by the IANA.

payload: http://www.w3.org/ns/dcat#mediaType

substructures:
  "https://gedcom.io/terms/v7/MEDI": "{0:1}"

superstructures:
  "https://gedcom.io/terms/v7/FILE": "{1:1}"
  "https://gedcom.io/terms/v7/FILE-TRAN": "{1:1}"
...

```
