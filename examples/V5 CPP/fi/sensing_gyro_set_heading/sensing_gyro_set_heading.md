category: sensing  
signature: GYRO.setHeading(90, degrees);  
device_class: gyro  
description: Sets the Gyroscopic (Gyro) sensor's current position to the value provided. 

# Gyro aseta ajosuunta

Asettaa Gyroscopic (Gyro) sensorin uuden nykyisen ajosuunnan. 

```cpp
Gyro.setHeading(0, degrees);
```

## Miten käytetään

`Gyro.setHeading();` komennossa voi asettaa gyrona rvoksi minkä tahansa myötäpäivvä asennon. Tyypillisesti ajosuunta nollataan kesken ajoa.

`Gyro.setHeading();` hyväksyy desimaali- ja kokonaislukuja.

```cpp
Gyro.setHeading(0, degrees);
```

<advanced>
</advanced>