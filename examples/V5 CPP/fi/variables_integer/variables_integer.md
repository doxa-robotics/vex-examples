category: variables 
signature: variables_intergers
description: Sets a variable to a `int` type.

# Kokonaisluku muuttuja

Määrittelee kokonaislukumuuttujan ja antaa sille nimen ja alkuarvon.

`int myNumber = 10;`

## Miten käytetään

Anna yksikäsitteinen ja kuvaava nimi muuttujalle.

`int driveTime = 60;`

Anna muuttujalle alkuarvo. Muuttujan arvo voi olla jonkun sensorin antama arvo tai laskutoimituksen tulos edellyttäen, että tulos on oikeaa **tyyppiä**.

```cpp
int lowBatteryLifeWarning = Brain.Battery.capacity(percent);
```

## Esimerkki

Tässä esimerkissä VEX V5 etäisyysanturin mittaama etäisyysarvo sijoitetaan "myVariable" muuttujaan ja sen jälkeen "myVariable" sijoitetaan ajopelin nopeudeksi.

```cpp
int myVariable = Distance7.objectDistance(inches);

Drivetrain.setDriveVelocity(myVariable, percent);
```

<advanced>
</advanced>