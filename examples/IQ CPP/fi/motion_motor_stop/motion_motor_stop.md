category: motion  
signature: Motor.stop();  
device_class: motor  
description: Stops a motor.  

# Pysäytä Moottori

Pysäyttää moottorin.

```cpp
Motor.stop();
```

## Miten käytetään

Alkuosa komentoa kertoo, mikä moottori on valittu.
```cpp
ClawMotor.stop();
ArmMotor.stop();
``` 

## Esimerkki

Esimerkissä Kouramoottori ClawMotor pysäytetään kun 3 sekuntia on kulunut eteenpäin pyörimisestä.

```cpp
ClawMotor.spin(forward);
wait(3, seconds);
ClawMotor.stop();
```

<advanced>
</advanced>