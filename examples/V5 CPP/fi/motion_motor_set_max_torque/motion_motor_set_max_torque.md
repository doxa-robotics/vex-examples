category: motion  
signature: MOTOR.setMaxTorque(50, percent);
device_class: motor  
description: Sets the V5 Smart Motor's max torque.  

# Aseta maksimi moottorin vääntö

Asettaa V5 älymoottorin masimi väännön.

```cpp
Motor.setMaxTorque(value, units);
``

## Miten käytetään

Komento sallii arvot välillä 0% - 100%.

Maksimi moottorin vääntö -komento sallii desimaali- ja kokonaislukuja sekä numeerisia arvoja.

## Esimerkki

Esimerkissä kouramoottori liikkuu asentoon 40 astetta maksimi moottorin väännöllä 20 %, jolloin tarttuessa esineeseen moottori ei riko esinettä.


```cpp
ClawMotor.setMaxTorque(20, percent);
ClawMotor.spinToPosition(40, degrees);
```

<advanced>
</advanced>