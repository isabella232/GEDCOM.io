---
title: FILE
permalink: /terms/v7/FILE.html
layout: none
redirect-from:
  - /terms/v7/FILE
...

```

%YAML 1.2
---
type: structure

uri: https://gedcom.io/terms/v7/FILE

standard tag: FILE

descriptions:
  - File reference
  - |
    A reference to an external file. Syntactically, the payload is a URI
    reference as defined by RFC 3986, or a valid URL string as defined by the
    WHATWG URL specification. That is, it can be an absolute or relative URL,
    optionally with a fragment string. However, only the following URL types
    are used:
    
    -   A URL with scheme ftp, http, or https refers to a web-accessible file.
    
    -   A URL with scheme file refers to a machine-local file as defined by RFC
        8089. Machine-local files must not be used in FamilySearch GEDZIP nor
        when sharing datasets on the web or with unknown parties, but may be
        used for close collaboration between parties with known similar file
        structures.
    
    -   A URI reference with all of the following:
    
        -   no scheme
        -   not beginning with / (U+002F)
        -   not containing any path segments equal to .. (U+002E U+002E)
        -   not containing a reverse solidus character (U+005C \) or banned
            character, either directly or in escaped form
        -   no query or fragment
    
        refers to a local file. If the dataset is part of a GEDZIP file, the
        URL of the local file is a zip archive filename; otherwise, the URL of
        a local file is resolved with base equal to the directory containing
        the dataset.
    
        It is recommended that local files use the directory prefix media/, but
        doing so is not required.
    
        For compatibility with GEDZIP and related formats, it is recommended
        that the following FILE payloads not be used:
    
        -   gedcom.ged
        -   MANIFEST.MF
        -   any URL beginning META-INF/
    
    The meaning of a FILE payload with any format not listed above is not
    defined by this version of the specification, but may be defined in a
    subsequent version.

payload: http://www.w3.org/2001/XMLSchema#string

substructures:
  "https://gedcom.io/terms/v7/FILE-TRAN": "{0:M}"
  "https://gedcom.io/terms/v7/FORM": "{1:1}"
  "https://gedcom.io/terms/v7/TITL": "{0:1}"

superstructures:
  "https://gedcom.io/terms/v7/record-OBJE": "{1:M}"
...

```
