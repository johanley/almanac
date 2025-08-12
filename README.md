# Islander's Almanac

Errata and background info for the Islander's Almanac. 

## Known Errors

### Charlottetown 2026 
No known errors.

## Background Info

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

### Calculation of Weather Normals
The Islander's Almanac uses the following algorithm for calculating weather normals,  described here using an example.

*What is the normal high temperature for Charlottetown for March 10?*

- use daily-high data for the *Charlottetown A* weather station (the airport) over a long period; let's say there are 51 years of data
- use plus-minus 3 days on either side of March 10, that is, *March 7 to March 13 inclusive*
- gather together all the daily highs for those 7 days, across all 51 years (*7 x 51 = 357* readings)
- sort/list the 357 readings from lowest to highest
- select the reading in the middle of the list (the median value) as the normal high temperature for March 10 for Charlottetown
- to find the *80%-range* for the data, drop the top and bottom 10% of the values in the list; this is a measure of the spread in the data

This technique uses *median* values, not *average/mean* values. This avoids some minor skew from extreme values.

(Note as well: data for leap days February 29 are coerced into data for March 1).

This technique is not the same as the technique used by Environment Canada, so you will see small differences with their weather normals.

The idea of using plus-minus 3 days of data is used to smooth the data.


