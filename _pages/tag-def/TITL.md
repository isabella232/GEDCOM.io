---
title: TITL
permalink: /terms/v7/TITL.html
layout: none
redirect-from:
  - /terms/v7/TITL
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/TITL

standard tag: TITL

descriptions:
  - Title
  - |
    The title, formal or informal, of the superstructure.
    
    A published work, such as a book, might have a title plus the title of the
    series of which the book is a part. A magazine article would have a title
    plus the title of the magazine that published the article.
    
    For an unpublished work, including most digital files, titles should be
    descriptive and appropriate to the work.
    
    -   The TITL of a letter might include the date, the sender, and the
        receiver.
    -   The TITL of a transaction between a buyer and seller might have their
        names and the transaction date.
    -   The TITL of a family Bible containing genealogical information might
        have past and present owners and a physical description of the book.
    -   The TITL of a personal interview would cite the informant and
        interviewer.
    
    Some sources may have a citation text that cannot readily be represented
    using the SOURCE_RECORD substructures AUTH, PUBL, REPO, and so on. In such
    cases, the entire citation text may be presented as the payload of the
    SOUR.TITL.
  - title
  - A formal designation used by an individual in connection with positions of
    royalty or other social status, such as Grand Duke.

payload: http://www.w3.org/2001/XMLSchema#string

substructures: []

superstructures:
  "https://gedcom.io/terms/v7/FILE": "{0:1}"
  "https://gedcom.io/terms/v7/OBJE": "{0:1}"
  "https://gedcom.io/terms/v7/record-SOUR": "{0:1}"
...

```
