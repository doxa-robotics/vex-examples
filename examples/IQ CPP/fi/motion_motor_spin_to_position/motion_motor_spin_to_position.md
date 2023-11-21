category: motion  
signature: Motor.spinToPosition(90, degrees);  
device_class: motor  
description: Spins the motor to a position.  

# Pyöritä Moottori Asentoon

Pyörittää moottorin tiettyyn asentoon.

```cpp
Motor.spinToPosition(rotation, units);
```

## Miten käytetään

`Motor.spinToPosition` pyörittää VEX IQ Älymoottorin tiettyy haluttuun asentoon nykyisestä asennosta, `Motor.spinToPosition` päättää mihin suuntaan pitää pyöriä.

`Motor.spinToPosition` hyväksyy numeerisia arvoja pyörimiselle `rotation`.

Voit valita pyörimisen yksiköksi jokoa **asteita** tai **kierroksia**. 

`Motor.spinToPosition` komento blokkaa muut komennot kunnes se on saavuttanut halutun asennon.

## Parametrit

Voit valita parametriarvon `epätosi` viimeiseksi arvoksi, jolloin 'Motor.spinToPosition` ei estä seuraavaa komentoa ennen kuin sen pyörimisliike on valmis.

```cpp
Motor.spinToPosition(360, degrees, false);
```

<advanced>
</advanced>