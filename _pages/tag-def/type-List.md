---
title: type-List
permalink: /terms/v7/type-List.html
layout: none
redirect-from:
  - /terms/v7/type-List
...

```

%YAML 1.2
---
type: datatype

uri: https://gedcom.io/terms/v7/type-List

descriptions:
  - |
    A list is a meta-syntax representing a sequence of values with another
    datatype. Two list datatypes are used in this document: List:Text and
    List:Enum. Lists are serialized in a comma-separated form, delimited by a
    comma (U+002C ,) and any number of spaces (U+0020) between each item. It is
    recommended that a comma-space pair (U+002C U+0020) be used as the
    delimiter.
    
        List      = listItem *(listDelim listItem)
        listItem  = "" / nocommasp / nocommasp *nocomma nocommasp
        listDelim = *D "," *D
        nocomma   = %x09-2B / %x2D-10FFFF
        nocommasp = %x09-1D / %x21-2B / %x2D-10FFFF
    
        List-Text = List
        List-Enum = Enum *(listDelim Enum)
    
    If valid for the underlying type, empty strings may be included in a list
    by having no characters between delimiters.
    
    A List:Text with value “, , one, more,” has 5 Text-type values: 2 empty
    strings, the string “one”, the string “more”, and 1 more empty string.
    
    There is no escaping mechanism to allow lists of entries that begin or end
    with spaces or that contain comma characters.
    
    The URI for the List:Text datatype is
    https://gedcom.io/terms/v7/type-List#Text.
    
    The URI for the List:Enum datatype is
    https://gedcom.io/terms/v7/type-List#Enum.
...

```
