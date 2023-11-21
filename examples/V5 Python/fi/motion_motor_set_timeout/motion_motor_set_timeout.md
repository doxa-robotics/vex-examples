category: motion  
signature: motor.set_timeout(TIME, SECONDS)  
description: Sets a time limit for the V5 Smart Motor movement commands.

# Aseta moottorille odotusaika

Asettaa moottorille odotusajan seuraavalle liikkeelle.

```don 
motor.set_timeout(TIME, SECONDS)
```

## Miten käytetään

Aseta moottorille odotusaika antaa moottorille aika-rajan , jona aikana sen pitää suorittaa meneillään oleva komento loppuun. Tällä estetään ohjelman suorituksen loppuminen kesken, kun moottori ei saavuta tavoitetta. 

Esimerkinä aikarajan tarpeelle Käsi - tai Kouramoottorille on, että sen kääntymisen estää sen rakenteen mekaaniset rajat tai muu este.

## Esimerkki

Tässä esimerkissä aikaraja komennolle `spin_to_position` on 2 sekuntia.

Jos moottori ei tavoita 270 asteen kääntymsitavoitetta 2 sekunin aikana, moottori pysäytetään.

```don
claw_motor.set_timeout(2, SECONDS)
claw_motor.spin_to_position(270, DEGREES)
```

<advanced>
</advanced>
