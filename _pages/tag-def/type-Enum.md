---
title: type-Enum
permalink: /terms/v7/type-Enum.html
layout: none
redirect-from:
  - /terms/v7/type-Enum
...

```

%YAML 1.2
---
type: datatype

uri: https://gedcom.io/terms/v7/type-Enum

descriptions:
  - |
    An enumeration is a selection from a set of options. They are represented
    as a string matching the same production as a tag.
    
        Enum    = Tag
    
    Each structure type with an enumeration payload also defines specific
    payload values it permits. These permitted payloads match production stdTag
    and should each have a defined URI. Payload values that match production
    extTag are always permitted in structures with an enumeration payload and
    have their URI defined by the schema.
    
    Each enumeration value has a distinct meaning as identified by its
    corresponding URI.
    
    The URI for the Enum datatype is https://gedcom.io/terms/v7/type-Enum.
...

```
