---
title: ROLE
permalink: /terms/v7/ROLE.html
layout: none
redirect-from:
  - /terms/v7/ROLE
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/ROLE

standard tag: ROLE

descriptions:
  - Role
  - |
    An enumerated value indicating what role this person played in an event or
    person’s life.
    
    The following indicates a child’s birth record as the source of the
    mother’s name:
    
        0 @I1@ INDI
        1 NAME Mary //
        2 SOUR @S1@
        3 EVEN BIRT
        4 ROLE MOTH
    
    The following indicates that a person’s best friend was a witness at their
    baptism:
    
        0 @I2@ INDI
        1 ASSO @I3@
        2 ROLE FRIEND
        3 PHRASE best friend
        1 BAPM
        2 ASSO @I3@
        3 ROLE WITN

payload: https://gedcom.io/terms/v7/type-Enum

enumeration values:
  CHIL: https://gedcom.io/terms/v7/enum-CHIL
  CLERGY: https://gedcom.io/terms/v7/enum-CLERGY
  FATH: https://gedcom.io/terms/v7/enum-FATH
  FRIEND: https://gedcom.io/terms/v7/enum-FRIEND
  GODP: https://gedcom.io/terms/v7/enum-GODP
  HUSB: https://gedcom.io/terms/v7/enum-HUSB
  MOTH: https://gedcom.io/terms/v7/enum-MOTH
  MULTIPLE: https://gedcom.io/terms/v7/enum-MULTIPLE
  NGHBR: https://gedcom.io/terms/v7/enum-NGHBR
  OFFICIATOR: https://gedcom.io/terms/v7/enum-OFFICIATOR
  OTHER: https://gedcom.io/terms/v7/enum-OTHER
  PARENT: https://gedcom.io/terms/v7/enum-PARENT
  SPOU: https://gedcom.io/terms/v7/enum-SPOU
  WIFE: https://gedcom.io/terms/v7/enum-WIFE
  WITN: https://gedcom.io/terms/v7/enum-WITN

substructures:
  "https://gedcom.io/terms/v7/PHRASE": "{0:1}"

superstructures:
  "https://gedcom.io/terms/v7/ASSO": "{1:1}"
  "https://gedcom.io/terms/v7/SOUR-EVEN": "{0:1}"
...

```
