# placetime
A new, better time.

# Formula
```
Placetime(Lon) = ((placeAdjust(Lon) + sunPos) % secondsInDay) / secondsInDay

Where:
    secondsInDay = 86400
    placeAdjust(Lon) = secondsInDay / 2 * Lon / 180
    sunPos = Date.Now() / 1000  // relative to UTC
```

## Calculation
How many meters to the east/west to cause 0.00001 change in placetime?  
400.75 meters === 0.00001 * Earth Circumference in meters
