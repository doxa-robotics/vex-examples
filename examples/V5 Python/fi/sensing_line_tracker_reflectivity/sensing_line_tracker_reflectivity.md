category: sensing  
signature: line_tracker.reflectivity(PERCENT)
description: Reports the amount of light reflected using the Line Tracker sensor.

# Viivanseuranta heijastus

Antaa valon määrän, joka heijastuu Viivanseuranta-sensoriin.

```don
line_tracker.reflectivity(PERCENT)
```

## Miten käytetään

Vaaleat pinnat heijastaa paremmin valoa kuin tummat pinnat ja myös heijastusarvo vaaleilla on suurempi.

Tummat pinnat heijastaa valoa huonommin ja myös heijastusarvo on pieni.

Yksikkönä käytyetään`PERCENT`(prosenttia) ja komento palauttaa kokonaislukuarvon välillä **0% - 100%**.

<advanced>
</advanced>
