category: motion  
signature: MOTOR.setStopping(brake);  
device_class: motor  
description: Sets the V5 Smart Motors brake mode.  

# Moottorin pysähtymistapa

Asettaa V5 moottorin pysähtymistavan. 

```cpp
Motor.setStopping(brakeType);
```

## Miten käytetään

`MODE` parametrissa voi asettaa jonkun seuraavista tavoista:

* BRAKE: moottori pysähtyy heti.
* COAST: moottori pysähtyy vaiheittain.
* HOLD: moottori pysähtyy herti ja pitää paikan vaikka joku ulkoinen voima sitä yrittää siirtää esim painovoima.

Moottorin pysähtymsistapa säilyy ohjelman läpi ellei uusi komento sitä muuta.

## Esimerkki

Esimerkissä moottori pyörii eteenpäin 90 astetta (käsi nousee) ja sen jälkeen mooorroti pysähtyy 'hold' asentoon.

```cpp
ArmMotor.setStopping(hold);
ArmMotor.spinFor(90, degrees);
```

<advanced>
</advanced>