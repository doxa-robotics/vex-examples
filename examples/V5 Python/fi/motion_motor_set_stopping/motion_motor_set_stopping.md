category: motion  
signature: motor.set_stopping(BRAKE)  
description: Sets the behavior of the V5 Smart Motor once it stops moving.

# Moottorin pysähtymistapa

Asettaa V5 moottorin pysähtymistavan.

```don
motor.set_stopping(MODE)
```

## Miten käytetään

`MODE` parametrissa voi asettaa jonkun seuraavista tavoista:

* BRAKE: moottori pysähtyy heti.
* COAST: moottori pysähtyy vaiheittain.
* HOLD: moottori pysähtyy herti ja pitää paikan vaikka joku ulkoinen voima sitä yrittää siirtää esim painovoima.

Moottorin pysähtymsistapa säilyy ohjelman läpi ellei uusi komento sitä muuta.

## Esimerkki

Esimerkissä moottori pyörii eteenpäin 90 astetta (käsi nousee) ja sen jälkeen mooorroti pysähtyy 'hold' asentoon.

```don
arm_motor.set_stopping(HOLD)
arm_motor.spin_for(FORWARD, 90, DEGREES)
```

<advanced>
</advanced>
