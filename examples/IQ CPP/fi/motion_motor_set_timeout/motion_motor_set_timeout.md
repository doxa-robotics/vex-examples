category: motion  
signature: Motor.setTimeout(1, seconds);  
device_class: motor  
description: Sets the Motor's timeout to stop if a blocking command never reaches its target.  

# Moottori Aseta suoritusaika

Asettaaa moottorille suoritusajan katon, kuinka kauan se pyörii , jos se ei saavuta haluttua pyörimismäärää sitä ennen.  

```cpp
Motor.setTimeout(time, seconds);
```

## Miten käytetään

`Motor.setTimeout` komentoa käytetään tilanteissa, että halutaan varmistua että ohjelma jatkuu seuraavalla komennolla vaikka pyörimiselle asetettua tavoitetta ei saavuteta. 

Tällainen moottori on esimerkiksi koura- tai nostomoottori, jonka liikkeen voi pysäyttää robotin mekaniikan rakenne tai kouraan otettava esine.

Aikaraja annetaan yksikössä **seconds** (sekuntia).

## Esimerkki

Esimerkissä `Motor.spinToPosition` komento rajaa pyörimisajan arvoon 2 sekuntia ellei kouramoottori nimeltään ClawMotor saavuta asentoa 270 astetta. 

Sen jälkeen käsimoottori ArmMotor pyörii asentoon 90 astetta.

```cpp
ClawMotor.setTimeout(2, seconds);
ClawMotor.spinToPosition(270, degrees);
ArmMotor.spinToPosition(90, degrees);
```

<advanced>
</advanced>