category: motion  
signature: MOTOR.setTimeout(1, seconds);  
device_class: motor  
description: Sets the V5 Smart Motor's timeout to stop if a blocking command never reaches its target.  

# Aseta moottorille odotusaika

Asettaa moottorille odotusajan seuraavalle liikkeelle.

```cpp
Motor.setTimeout(time, seconds);
```

## Miten käytetään

Aseta moottorille odotusaika antaa moottorille aika-rajan , jona aikana sen pitää suorittaa meneillään oleva komento loppuun. Tällä estetään ohjelman suorituksen loppuminen kesken, kun moottori ei saavuta tavoitetta. 

Esimerkinä aikarajan tarpeelle Käsi - tai Kouramoottorille on, että sen kääntymisen estää sen rakenteen mekaaniset rajat tai muu este.

## Esimerkki

Tässä esimerkissä aikaraja komennolle `spin_to_position` on 2 sekuntia.

Jos moottori ei tavoita 270 asteen kääntymsitavoitetta 2 sekunin aikana, moottori pysäytetään.

```cpp
ClawMotor.setTimeout(2, seconds);
ClawMotor.spinToPosition(270, degrees);
ClawMotor.spinToPosition(0, degrees);
```

<advanced>
</advanced>