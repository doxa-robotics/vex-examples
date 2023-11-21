category: sensing  
signature: Gyro.setRotation(rotation, degrees);  
device_class: gyro  
description: Sets the Gyroscopic (Gyro) sensor's current rotation to the value provided. 

# Gyro Aseta kiertokulma

Asettaa VEX IQ Gyro sensorin kiertokulmalle tietyn arvon. 

```cpp
Gyro.setRotation(rotation, degrees);
```

## Miten käytetään

`Gyro.setRotation` komentoa voi käyttää, kun haluaa asettaa ajopelin kääntymiskulman tiettyyn positiiviseen (vastapäivään kierto) tai negatiiviseen (myötäpäivään kierto) arvoon.

`Gyro.setRotation` hyväksyy positiiviset ja negatiiviset desimaali- ja kokonaisluvut.

## Esimerkki

Esimerkissä Gyron kiertokulma asetetaan arvoon -45 astetta.

```cpp
Gyro.setRotation(-45, degrees);
```

<advanced>
</advanced>