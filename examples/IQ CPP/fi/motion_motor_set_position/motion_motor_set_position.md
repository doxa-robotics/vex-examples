category: motion  
signature: Motor.setPosition(0, degrees);  
device_class: motor  
description: Sets the Motor's encoder to a position.  

# Moottori Aseta asentoon

Asettaa VEX IQ Moottorin pyörimismitan encoder-arvon uudelleen haluttuun arvoon.

```cpp
Motor.setPosition(position, units);
```

## Miten käytetään

`Motor.setPosition` komennolla pyörimismitta/asento voidaan laittaa mihin haluttuun asentoarvoon tahansa kesken ohjelman.

Komennon ensimmäinen osa on valittu moottori.

```cpp
ClawMotor.setPosition(0, degrees);
ArmMotor.setPosition(90, degrees);
```

Tavallisesti `Motor.setPosition` komennossa nollataan pyörimisen asentomuisti.

Komennossa voi käyttää `yksikkönä` joko **degrees** (asteita) tai **turns** (kierroksia).

## Esimerkki

Esimerkissä kouramoottorin ClawMotor asennoksi (encoder) asetetaan 50 astetta.

```cpp
ClawMotor.setPosition(50, degrees);
```

<advanced>
</advanced>