# Islander's Almanac

Errata and background info for the *Islander's Almanac*. 

Contact the author: johnohanley85@gmail.com

## Known Errors

### Charlottetown 2026 
No known errors.


## Background Info


### Calculation of Weather Normals
The *Islander's Almanac* uses the following algorithm for calculating weather normals,  described here using an example.

*What is the normal high temperature for Charlottetown for March 10?*

- use daily-high temperature data for the *Charlottetown A* weather station (the airport) over a long period; let's say there are 51 years of data
- use plus-minus 3 days on either side of *March 10*, that is, *March 7 to March 13 inclusive*
- gather together all the daily highs for those 7 days, across all 51 years (*7 x 51 = 357* readings)
- sort/list the 357 readings from lowest to highest
- select the reading in the middle of the list (the *median* value) as the normal high temperature for March 10 for Charlottetown
- to find the *80%-range* for the daily high at Charlottetown on March 10, drop the top and bottom 10% of the values in the sorted list; this is a measure of the spread in the data.
The daily high temperature value is in this range 80% of the time (in the given data set).


Note :
- this technique uses *median* values, not *average/mean* values. This avoids some minor skew from extreme values.
- data for leap days *February 29* are coerced into data for *March 1*.
- at the start and end of the year, the data is *wrapped around*: for *January 1*, plus-minus 3 days gives the date range *December 29 to January 4 inclusive*.
- the idea of using plus-minus 3 days of data is used to smooth the data.
- when the median value is not centered in the corresponding 80%-range, that means there's some skew in the data (which is useful to know).


**This technique is not the same as the technique used by Environment Canada, so you will see small differences with their weather normals.**


### Abbreviations
In the list of daily events, some cryptic abbreviations are used to make best use of the limited space.

Abbreviations used for occultations:
- `DD` disappearance at the dark limb of the Moon
- `DB` disappearance at the bright limb of the Moon
- `RD` reappearance at the dark limb of the Moon
- `RB` reappearance at the bright limb of the Moon

Abbreviations for some astronomical events:
- `IC` inferior conjunction of a planet with the Sun
- `SC` superior conjunction of a planet with the Sun
- `GE` greatest elongation of a planet from the Sun


### Missing Diagram for Jupiter
Some days have no diagram for the moons of Jupiter. 

Those are days for which Jupiter is too close to the Sun to be observed.


### Hour Angle of the Moon: high and low tides
The *hour angle* of an object in the sky is the number of hours since it was due south.
An hour angle of *2h* means an object was due south 2 hours ago.
An hour angle of *22h* means an object will be due south in 2 hours.

The idea is that, in many places (such as Charlottetown, on the south shore), the time of high or low tide is correlated fairly well with the hour angle of the Moon.
In some places, however, the correlation is poor (such as Stanhope, on the north shore).

