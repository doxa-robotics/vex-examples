category: motion  
signature: MOTOR.spin(forward);  
device_class: motor  
description: Spins a V5 Smart Motor in a direction until stopped.  

# Moottori pyörii

pyörittää V5 älymoottoria kunnes se pysäytetään.

```cpp
Motor.spin(directionType);
```

## Miten käytetään

`Motor.spin();` pyörittää V5 älymoottoria ikuisesti kunnes uusi komento sen pysäyttää tai ohjelman suoritus keskeytetään.

Käytä parametria `forward` kun haluat moottorin pyörivän eteenpäin.

```cpp
Motor.spin(forward);
```
Käytä parametria `reverse` kun haluat moottorin pyörivän taaksepäin.

```cpp
Motor.spin(reverse);
```

<advanced>
</advanced>