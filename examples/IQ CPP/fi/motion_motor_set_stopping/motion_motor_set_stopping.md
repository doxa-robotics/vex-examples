category: motion  
signature: Motor.setStopping(brake);  
device_class: motor  
description: Sets the Motors brake mode.  

# Moottori Aseta pysähtymistapa

Asettaa tarkemmin miten VEX IQ Älymoottori pysähtyy.

```cpp
Motor.setStopping(brakeType);
```

## Miten käytetään

Komennon ensimmäinen osa on nimetyn moottorin nimi.

```cpp
ClawMotor.setStopping(brake);
ArmMotor.setStopping(hold);
```

Määrittele moottorin pysähdystapa:

- **brake** pysähtyy heti
- **coast** pysähtyy hitaasti rullaten
- **hold** pysähtyy heti (jarrut lukossa) ja jää asentoon, vaikka sitä yritetään ulkoisesti liikuttaa.

`Motor.setStopping` vaikuttaa ohjelman jatkossa jokaisessa `Motor.stop` komennossa ellei sitä myöhemmin muuteta.

## Esimerkki

Käsimoottori ArmMotor pyörii eteenpäin 90 astetta ja vastustaa lukkojarrutuksella muita voimia (maan vetovoima) ja pysyy lukitttuna loppuasennossa.

```cpp
ArmMotor.setStopping(hold);
ArmMotor.spinFor(forward, 90, degrees);
```

<advanced>
</advanced>