---
title: RIN
permalink: /terms/v7/RIN.html
layout: none
redirect-from:
  - /terms/v7/RIN
...

```

%YAML 1.2
---
type: legacy

uri: https://gedcom.io/terms/v7/RIN

descriptions:
  - Record ID Number
  - |
    This URI is defined to support conversion from GEDCOM 5.5.1 to FamilySearch
    GEDCOM 7.0 and beyond. It is intended for use as the
    https://gedcom.io/terms/v7/TYPE of an 
    https://gedcom.io/terms/v7/EXID replacing 5.5.1's RIN structure.

    GEDCOM 5.5 and 5.5.1 defined RIN as follows:
    
    > A unique record identification number assigned to the record by the
    > source system. This number is intended to serve as a more sure means of
    > identification of a record for reconciling differences in data between
    > two interfacing systems.
    
    URLs beginning https://gedcom.io/terms/v7/RIN are used to represent
    such source systems if they did not have a dedicated URI. The fragment
    identifer of this URI (the part after the #) represents how the source
    system was identified in the 5.5 or 5.5.1 file's header; the payload of the
    EXID is the record identifier within that resource. If there is no fragment
    identifier, the EXID was an RIN given without a source system identifier.
    
    It is recommend that the 5.5.1 structure
    
        2 RIN 123abc
    
    in a file with HEAD.SOUR line value "XYZ"
    be converted to 7.0 structures
    
        2 EXID 123abc
        3 TYPE https://gedcom.io/terms/v7/RIN#XYZ

...

```
