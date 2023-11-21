category: motion  
signature: MOTOR.stop();  
device_class: motor  
description: Stops the V5 Smart Motor.  

# Pysäytä moottori

Pysäyttää moottorin.

```cpp
Motor.stop();
```

## Miten käytetään

`Motor.stop();` komento pysäyttää moottorin. Komennolla `Motor.setStopping();` voit asettaa pysähtymsitavan  `coast` (pysähdy heti) , `brake` (hitaasti jarruttaen), tai `hold` (pysähdy heti ja pidä asento).

## Esimerkki

Esimerkissä moottori pyörii 3 sekuntia ennen pysähtymistä.

```cpp
ClawMotor.spin(forward);
wait(3, seconds);
ClawMotor.stop();
```

<advanced>
</advanced>