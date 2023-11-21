category: sensing  
signature: MOTOR.isDone()  
device_class: motor  
description: Reports if the V5 Smart Motor has completed its movement.

# Mooottori on pysähtynyt?

raportoi onko moottori suorittanut loppuun liikkeensä.


```cpp
Motor.isDone()

## Miten käytetään

Komentoa käytetään yleensä muiden komentojen sisällä mm tulosta -komennossa tai toistorakenteiden ehdoissa

`Motor.isDone` antaa arvon **tosi**, kun tietty moottori on pysähtynyt.

`Motor.isDone` antaa arvon **epätosi**, kun tietty moottori ei ole suorittanut liikettä loppuun.

```cpp
waitUntil(ClawMotor.isDone());
```
<advanced>
</advanced>