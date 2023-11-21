category: sensing  
signature: GYRO.setRotation(90, degrees);  
device_class: gyro  
description: Sets the 3-Wire Gyro Sensor's angle of rotation to the value provided  

# Gyro Aseta kierrosaste

Asettaa 3-Lanka Gyro Sensorin kierroskulman haluttuun arvoon.

```cpp
Gyro.setRotation(0, degrees);
```

## Miten käytetään

Gyro.setRotation();` komento voidaan asettaa ajopelin kulmaksi minkä tahansa positiivisen (myötäpäivään) tai negatiivisen (vastapäivään) luvun kulman arvoksi.

`Gyro.setRotation();` hyväksyys ekä positiivisia että negatiivisia kokonais- ja desimaalilukuja.

```cpp
Gyro.setRotation(270, degrees);
Gyro.setRotation(-270, degrees);
```

<advanced>
</advanced>
