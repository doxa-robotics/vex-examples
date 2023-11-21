category: control  
signature: if condition: \n\tpass\nelse:\n\tpass  
description: Used to decide if one statement will execute or another will if the first statement is not true.

# Jos/muuten

Ohjauslause, joka suorittaa If -haaran, jos ehto on 'true' (tosi) ja Else -haaran jos ehto on 'false' (epätosi). 

```don
if condition:
    pass
else:
    pass

```

## Miten käytetään

'if` komento on ehto , joka saa joko arvon **True** tai **False**. Voit yhdistää ehtoihin useamman loogisen operaattorin `and`, `or`, and `not`. 

Jos ehto saa arvon **True**, `if ehdon:` haara suoritetaan. Jos ehto saa arvon **False**, `else:` haaran komennot suoritetaan.

Komentokoodi `if` ja `else` haarassa komennot on sisennetty 4 tyhjällä merkillä.

if/else` komennossa ei saa olla tyhjiä rivejä vaan tyhjä korvataan komennolla `pass`. 

## Esimerkki

Tämä `if/else` koodi ajaa robottia eteenpäin, jos muuttuja my_variable saa arvon 1. Jos arvo ei ole 1, ajetaan taaksenpäin. 

```don
if (my_variable == 1):
    drivetrain.drive(FORWARD)
else:
    drivetrain.drive(REVERSE)
```

<advanced>
</advanced>
