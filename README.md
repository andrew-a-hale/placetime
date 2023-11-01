# placetime
A new, better time.

# Formula
Placetime Formula = ((placeAdjust + sunPositionInSecondRelativeLonZero) % secondsInDay) / secondsInDay
where:
    secondsInDay = 86400
    placeAdjust(Lon) = secondsInDay / 2 * Lon / 180
    sunPositionInSecondRelativeLonZero = Date.Now() / 1000

## Calculation
How many meters to the east/west to cause 0.00001 change in placetime? 400.75 meters === 0.00001 * Earth Circumference in meters
