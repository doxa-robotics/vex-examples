category: sensing  
signature: Drivetrain.velocity(units)  
device_class: drivetrain
description: Reports the current velocity of the Drivetrain.

# Ajopelin Nopeus

Raportoi ajopelin nykyisen nopeuden.

```cpp
Drivetrain.velocity(units)
```

## Miten käytetään
`Drivetrain.velocity` palauttaa desimaaliluvun (*double*), kun se raportoi ajopelin nykyisen nopeuden. 

`Drivetrain.velocity` palauttaa arvon väliltä **-100% - 100%**, jos yksikkönä käytetään prosenttia **percent**.

`Drivetrain.velocity` yksikkönä voi olla myös **rpm** (kierrosta per minuutti).

Negatiiviset lukuarvot tarkoittavat, että ajopeli liikkuu taaksepäin.

## Esimerkki

Esimerkissä tulostetaan ajopelin nopeus (prosentteina) VEX IQ Aivojen näytölle.

```cpp
Brain.Screen.print("%f", Drivetrain.velocity(percent));
```

<advanced>
</advanced>