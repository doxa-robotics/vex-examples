category: control  
signature: break;  
description: Exits a repeating loop immediately.

# Keskeytä

Komennolla hypätään pois toistorakenteesta.
```cpp
break;
```

## Miten käytetään

Kun lisätään `break` kommento johonkin kohtaan toistorakennetta, se aiheuttaa hypyn pois silmukasta toiston jälkeiseen seuraavaan komentoon. 

## Esimerkki

esimerkissä ajataan eteenpäin ja ja tarkistetaan , onko `bumper` törmäysanturia painettu.

Jos näyttöä on painettu on kosketettu, 'break` komento aiheuttaa hypyn pois silmukan suorituksesta ja ajopeli pysähtyy.


```cpp
while (true) {
  Drivetrain.drive(forward);
  if(Brain.Screen.pressing()) {
    break;
  }
}

Drivetrain.stop();
```
<advanced>
</advanced>