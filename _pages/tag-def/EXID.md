---
title: EXID
permalink: /terms/v7/EXID.html
layout: none
redirect-from:
  - /terms/v7/EXID
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/EXID

standard tag: EXID

descriptions:
  - External Identifier
  - |
    An identifier for the subject of the superstructure. The identifier is
    maintained by some external authority; the authority owning the identifier
    is provided in the TYPE substructure; see EXID.TYPE for more.
    
    Depending on the maintaining authority, an EXID may be a unique identifier
    for the subject, an identifier for 1 of several views of the subject, or an
    identifier for the externally-maintained copy of the same information as is
    contained in this structure. However, unlike UID and REFN, EXID does not
    identify a structure; structures with the same EXID may have originated
    independently rather than by edits from the same starting point.

payload: http://www.w3.org/2001/XMLSchema#string

substructures:
  "https://gedcom.io/terms/v7/EXID-TYPE": "{0:1}"

superstructures:
  "https://gedcom.io/terms/v7/PLAC": "{0:M}"
  "https://gedcom.io/terms/v7/record-FAM": "{0:M}"
  "https://gedcom.io/terms/v7/record-INDI": "{0:M}"
  "https://gedcom.io/terms/v7/record-OBJE": "{0:M}"
  "https://gedcom.io/terms/v7/record-REPO": "{0:M}"
  "https://gedcom.io/terms/v7/record-SNOTE": "{0:M}"
  "https://gedcom.io/terms/v7/record-SOUR": "{0:M}"
  "https://gedcom.io/terms/v7/record-SUBM": "{0:M}"
...

```
