category: sensing  
signature: Drivetrain.isMoving()  
device_class: drivetrain  
description: Reports if the Drivetrain is currently moving.

# Ajopeli liikkuu

Antaa tiedon jatkaako ajoplei liikettä tällä hetkellä.

```cpp
Drivetrain.isMoving()
```

## Miten käytetään

Komennot, jotka palauttavat arvon voidaan sijoittaa toisten komentojen sisään kuten print -komennossa tao ohjauslauseissa ehtomuuttujien osana ja ilman puolipistettä.

Komento antaa arvon **true** jos ajopeli edelleen suorittaa komentoa `driveFor()` tai `turnFor()` , jossa on etäisyysmääre käytössä.

Komento antaa arvon **false** jos ajopeli on jo pysähtynyt .

**Note:** Tämä komento antaa aina vain arvon **false** jos liikettä tehdään komennoilla `drive()` tai `turn()`, jossa ei ole annettu matkaa/astemäärää.

```cpp
if (Drivetrain.isMoving()) {
    
} else {
    
}
```

<advanced>
</advanced>