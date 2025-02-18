---
title: type-Time
permalink: /terms/v7/type-Time.html
layout: none
redirect-from:
  - /terms/v7/type-Time
...

```

%YAML 1.2
---
type: datatype

uri: https://gedcom.io/terms/v7/type-Time

descriptions:
  - |
    Time is represented on a 24-hour clock (for example, 23:00 rather than
    11:00 PM). It may be represented either in event-local time or in
    Coordinated Universal Time (UTC). UTC is indicated by including a Z
    (U+005A) after the time value; event-local time is indicated by its
    absence.
    
        Time     =  hour ":" minute [":" second ["." fraction]] [%s"Z"]
    
        hour     = digit / ("0" / "1") digit / "2" ("0" / "1" / "2" / "3")
        minute   = ("0" / "1" / "2" / "3" / "4" / "5") digit
        second   = ("0" / "1" / "2" / "3" / "4" / "5") digit
        fraction = 1*digit
    
    The above grammar prohibits end-of-day instant 24:00:00 and leap-seconds.
    It allows both 02:50 and 2:50 as the same time.
    
    The URI for the Time datatype is https://gedcom.io/terms/v7/type-Time.
...

```
