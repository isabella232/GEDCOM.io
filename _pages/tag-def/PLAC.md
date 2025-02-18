---
title: PLAC
permalink: /terms/v7/PLAC.html
layout: none
redirect-from:
  - /terms/v7/PLAC
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/PLAC

standard tag: PLAC

descriptions:
  - Place
  - |
    The principal place in which the superstructure’s subject occurred,
    represented as a [List] of jurisdictional entities in a sequence from the
    lowest to the highest jurisdiction. As with other lists, the jurisdictions
    are separated by commas. Any jurisdiction’s name that is missing is still
    accounted for by an empty string in the list.
    
    The type of each jurisdiction is given in the PLAC.FORM substructure, if
    present, or in the HEAD.PLAC.FORM structure. If neither is present, the
    jurisdictional types are unspecified beyond the lowest-to-highest order
    noted above.
  - |
    Having an EXID without an EXID.TYPE substructure is deprecated. The meaning
    of an EXID depends on its EXID.TYPE. The cardinality of EXID.TYPE will be
    changed to {1:1} in version 8.0.
    
    A place, which can be represented in several ways:
    
    -   The payload contains a comma-separated list of region names, ordered
        from smallest to largest. The specific meaning of each element is given
        by the FORM substructure, or in the HEAD.PLAC.FORM if there is no FORM
        substructure. Elements should be left blank if they are unknown, do not
        apply to the location, or are too specific for the region in question.
    
        A record describing births throughout Oneida county could be recorded
        as
    
            0 @S1@ SOUR
            1 DATA
            2 EVEN BIRT
            3 PLAC , Oneida, Idaho, USA
            4 FORM City, County, State, Country
    
    -   The payload may be translated or transliterated into different
        languages or scripts using the TRAN substructure. It should use the
        same FORM as the payload.
    
    -   Global coordinates may be presented in the MAP substructure
    
    This specification does not support places where a region name contains a
    comma. An alternative system for representing locations is likely to be
    added in a later version.

payload: https://gedcom.io/terms/v7/type-List#Text

substructures:
  "https://gedcom.io/terms/v7/EXID": "{0:M}"
  "https://gedcom.io/terms/v7/LANG": "{0:1}"
  "https://gedcom.io/terms/v7/MAP": "{0:1}"
  "https://gedcom.io/terms/v7/NOTE": "{0:M}"
  "https://gedcom.io/terms/v7/PLAC-FORM": "{0:1}"
  "https://gedcom.io/terms/v7/PLAC-TRAN": "{0:M}"
  "https://gedcom.io/terms/v7/SNOTE": "{0:M}"

superstructures:
  "https://gedcom.io/terms/v7/ADOP": "{0:1}"
  "https://gedcom.io/terms/v7/ANUL": "{0:1}"
  "https://gedcom.io/terms/v7/BAPL": "{0:1}"
  "https://gedcom.io/terms/v7/BAPM": "{0:1}"
  "https://gedcom.io/terms/v7/BARM": "{0:1}"
  "https://gedcom.io/terms/v7/BASM": "{0:1}"
  "https://gedcom.io/terms/v7/BIRT": "{0:1}"
  "https://gedcom.io/terms/v7/BLES": "{0:1}"
  "https://gedcom.io/terms/v7/BURI": "{0:1}"
  "https://gedcom.io/terms/v7/CAST": "{0:1}"
  "https://gedcom.io/terms/v7/CHR": "{0:1}"
  "https://gedcom.io/terms/v7/CHRA": "{0:1}"
  "https://gedcom.io/terms/v7/CONF": "{0:1}"
  "https://gedcom.io/terms/v7/CONL": "{0:1}"
  "https://gedcom.io/terms/v7/CREM": "{0:1}"
  "https://gedcom.io/terms/v7/DATA-EVEN": "{0:1}"
  "https://gedcom.io/terms/v7/DEAT": "{0:1}"
  "https://gedcom.io/terms/v7/DIV": "{0:1}"
  "https://gedcom.io/terms/v7/DIVF": "{0:1}"
  "https://gedcom.io/terms/v7/DSCR": "{0:1}"
  "https://gedcom.io/terms/v7/EDUC": "{0:1}"
  "https://gedcom.io/terms/v7/EMIG": "{0:1}"
  "https://gedcom.io/terms/v7/ENDL": "{0:1}"
  "https://gedcom.io/terms/v7/ENGA": "{0:1}"
  "https://gedcom.io/terms/v7/FAM-CENS": "{0:1}"
  "https://gedcom.io/terms/v7/FAM-EVEN": "{0:1}"
  "https://gedcom.io/terms/v7/FAM-FACT": "{0:1}"
  "https://gedcom.io/terms/v7/FAM-NCHI": "{0:1}"
  "https://gedcom.io/terms/v7/FAM-RESI": "{0:1}"
  "https://gedcom.io/terms/v7/FCOM": "{0:1}"
  "https://gedcom.io/terms/v7/GRAD": "{0:1}"
  "https://gedcom.io/terms/v7/IDNO": "{0:1}"
  "https://gedcom.io/terms/v7/IMMI": "{0:1}"
  "https://gedcom.io/terms/v7/INDI-CENS": "{0:1}"
  "https://gedcom.io/terms/v7/INDI-EVEN": "{0:1}"
  "https://gedcom.io/terms/v7/INDI-FACT": "{0:1}"
  "https://gedcom.io/terms/v7/INDI-NCHI": "{0:1}"
  "https://gedcom.io/terms/v7/INDI-RELI": "{0:1}"
  "https://gedcom.io/terms/v7/INDI-RESI": "{0:1}"
  "https://gedcom.io/terms/v7/INDI-TITL": "{0:1}"
  "https://gedcom.io/terms/v7/INIL": "{0:1}"
  "https://gedcom.io/terms/v7/MARB": "{0:1}"
  "https://gedcom.io/terms/v7/MARC": "{0:1}"
  "https://gedcom.io/terms/v7/MARL": "{0:1}"
  "https://gedcom.io/terms/v7/MARR": "{0:1}"
  "https://gedcom.io/terms/v7/MARS": "{0:1}"
  "https://gedcom.io/terms/v7/NATI": "{0:1}"
  "https://gedcom.io/terms/v7/NATU": "{0:1}"
  "https://gedcom.io/terms/v7/NMR": "{0:1}"
  "https://gedcom.io/terms/v7/OCCU": "{0:1}"
  "https://gedcom.io/terms/v7/ORDN": "{0:1}"
  "https://gedcom.io/terms/v7/PROB": "{0:1}"
  "https://gedcom.io/terms/v7/PROP": "{0:1}"
  "https://gedcom.io/terms/v7/RETI": "{0:1}"
  "https://gedcom.io/terms/v7/SLGC": "{0:1}"
  "https://gedcom.io/terms/v7/SLGS": "{0:1}"
  "https://gedcom.io/terms/v7/SSN": "{0:1}"
  "https://gedcom.io/terms/v7/WILL": "{0:1}"
...

```
