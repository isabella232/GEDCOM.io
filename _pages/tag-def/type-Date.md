---
title: type-Date
permalink: /terms/v7/type-Date.html
layout: none
redirect-from:
  - /terms/v7/type-Date
...

```

%YAML 1.2
---
type: datatype

uri: https://gedcom.io/terms/v7/type-Date

descriptions:
  - |
    The date formats defined in this specification include the ability to store
    approximate dates, date periods, and dates expressed in different
    calendars.
    
    Technically, there are 3 distinct date datatypes:
    
    -   DateValue is a generic type that can express many kinds of dates.
    -   DateExact is used for timestamps and other fully-known dates.
    -   DatePeriod is used to express time intervals that span multiple days.
    
        DateValue   = date / DatePeriod / dateRange / dateApprox / ""
        DateExact   = day D month D year  ; in Gregorian calendar
        DatePeriod  = %s"FROM" D date [D %s"TO" D date]
                    / %s"TO" D date
                    / ""
    
        date        = [calendar D] [[day D] month D] year [D epoch]
        dateRange   = %s"BET" D date D %s"AND" D date
                    / %s"AFT" D date
                    / %s"BEF" D date
        dateApprox  = (%s"ABT" / %s"CAL" / %s"EST") D date
    
        dateRestrict = %s"FROM" / %s"TO" / %s"BET" / %s"AND" / %s"BEF"
                    / %s"AFT" / %s"ABT" / %s"CAL" / %s"EST" / %s"BCE"
    
        calendar = %s"GREGORIAN" / %s"JULIAN" / %s"FRENCH_R" / %s"HEBREW"
                 / extTag
    
        day     = Integer
        year    = Integer
        month   = stdTag / extTag  ; constrained by calendar
        epoch   = %s"BCE" / extTag ; constrained by calendar
    
    In addition to the constraints above:
    
    -   The allowable months and epochs are determined by the calendar.
    -   No calendar names, months, or epochs match dateRestrict.
    -   Extension calendars (those with extTag for their calendar) must use
        extTag, not stdTag, for months.
    
    An absent calendar is equivalent to the calendar GREGORIAN.
    
    The grammar above allows for dates to be preceded by various words. The
    meaning of these words is given as follows:
    
      Production   Meaning
      ------------ ----------------------------------------------------------------------
      FROM x       Lasted for multiple days, beginning on x.
      TO x         Lasted for multiple days, ending on x.
      BET xAFT x   Exact date unknown, but no earlier than x.
      AND xBEF x   Exact date unknown, but no later than x.
      ABT x        Exact date unknown, but near x.
      CAL x        x is calculated from other data.
      EST x        Exact date unknown, but near x; and x is calculated from other data.
    
    Known calendars and tips for handling dual dating and extension calendars
    are given in Appendix A: Calendars and Dates.
    
    DateValue and DatePeriod payloads may also be the empty string if no
    suitable form is known but a substructure (such as a PHRASE or TIME) is
    desired.
    
    Versions 5.3 through 5.5.1 allowed phrases inside DateValue payloads. Date
    phrases were moved to the PHRASE substructure in version 7.0. A current
    limitation, however, is that a phrase in the PHRASE substructure cannot
    specify a language, so if a non-default language is needed to correctly
    interpret the phrase two options exist:
    
    -   PHRASE can be used with a documented extension tag for the language, as
        discussed in https://gedcom.io/terms/v7/LANG.
    
    -   <<EVENT_DETAIL>>.SOUR.DATA.TEXT can be used instead along with a LANG
        substructure; this loses the connection with the date, but includes the
        language with a standard tag.
    
    As defined by the grammar above, every date must have a year. If no year is
    known, the entire date may be omitted.
    
    The following is an appropriate way to handle a missing year
    
        2 DATE
        3 PHRASE 5 January (year unknown)
    
    The URI for the DateValue datatype is https://gedcom.io/terms/v7/type-Date.
    
    The URI for the DateExact datatype is
    https://gedcom.io/terms/v7/type-Date#exact.
    
    The URI for the DatePeriod datatype is
    https://gedcom.io/terms/v7/type-Date#period.
...

```
