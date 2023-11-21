category: sensing  
signature: inertial.set_heading(0, DEGREES)
description: Sets the Inertial sensor's current heading position to a set value.

# Aseta Inertial -sensorin ajosuunta

Asettaa Inertial -sensorin ajosuunnalle arvon.

```don
inertial.set_heading(HEADING, DEGREES)
```

## Miten käytetään

`inertial.set_heading` komennolla voi asetaa Inertial Sensorin asennon mihin tahansa kellotaulun arvoon, tyypillisesti se nollataan tarpeen mukaan kesken ajoa.

`inertial.set_heading` komento sallii arvot välillä 0.0 - 359.99 astetta.

`inertial.set_heading` komento sallii desimaaliarvoja, kokonaislukuja ja sensoreiden numeerisia arvoja.


<advanced>
</advanced>
