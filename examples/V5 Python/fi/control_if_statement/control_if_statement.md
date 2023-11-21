category: control  
signature: if condition:\n\tpass  
description: Used to decide whether or not a statement will be executed  

# Jos

Ohjauslause, joka päättelee, suoritetaanko ehdon `condition` toiminnot.

```don
if condition:
    pass
    
```

## Miten käytetään

Korvaa sana `condition` Boolean lausekkeella, joka saa jokoa rvon `True` tai `False`. Jos totuusarvo on `True`, niin `if` ehdon komennot suoritetaan.

Lisää aina 4 tyhjää merkki **spacebar** näppäimellä `if` haaran komentojen edelle. 

`if` ehto ei saa olla tyhjä vaain lisää vähintään komento `pass` haaran komennoksi. 

## Esimerkki

`if` haaran komennot ssuoritetaan , jos `my_variable`= 1, jolloin robotti ajaa eteenpäin.

```don
if (my_variable == 1):
    drivetrain.drive(FORWARD)
```

<advanced>
</advanced>
