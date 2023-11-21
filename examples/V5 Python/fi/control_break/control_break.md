category: control  
signature: break  
description: Exits a repeating loop immediately.

# Keskeytä

Komennolla hypätään pois toistorakenteesta.

```don
break
```

## Miten käytetään

Kun lisätään `break` kommento johonkin kohtaabn toistorakennetta, se aiheutta hypyn pois siitä toiston jälkeiseen seuraavaan komentoon. 

## Esimerkki

esimerkissä ajataan eteenpäin ja ja tarkistetaan , onko `bumper` törmäysanturia painettu.

Jos törmäysanturia bumber on **pressed**, 'break` komento aiheuttaa hypyn pois silmukan suorituksesta ja ajopeli pysähtyy.

```don
while True:
    drivetrain.drive(FORWARD)
    if bumper.pressing():
        break
```
<advanced>
</advanced>
