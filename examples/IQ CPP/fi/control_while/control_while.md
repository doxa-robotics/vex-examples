category: control  
signature: control_while
description: A loop that repeats the code inside the curly brackets while the condition returns true. 

# Kun

Toistorakenne toistaa sen sisältämän koodin kun ehto **condition** on voimassa **true**.   

```cpp
while (condition) {
  // Koodi suoritetaan toistuvasti kun ehto on voimassa
}
```

## Miten käytetään

'Kun` toisto tutkii sen sisältämää ehtoa aina kierroksen alussa. 

Jos ehto on totta **true**, silmukan sisällä oleva koodi suoritetaan.

Jo ehto on epätosi **false**, silmuikan yli hypätään suorittemaan seuraaavaa komentoa.

`while` hyväksyy kaikki Boolean arvoiset esitykset, jotka antavat totuusarvot **true** tai **false** ehdossaan. Ehdot voivat olla myös vertailuoperaatioita tai mitä tahansa loogisia ehtolauseita.  

## Esimerkki

Esimerkissä ajopeli ajaa eteenpäin kun kello on käynyt alle 60 sekuntia.

Sen jälkeen ajopeli pysähtyy.

```cpp
while(Brain.Timer.value() < 60) {
  Drivetrain.drive(forward);
  wait(20, msec);
}

Drivetrain.stop();
```

<advanced>
</advanced>