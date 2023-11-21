category: control  
signature: if(true) { }  
description: Runs the code inside the if-statement's curly brackets, if the condition returns true. 

# Jos

Ohjauslause, joka päättelee, suoritetaanko ehdon `condition` toiminnot.


```cpp
if (condition) {

}
```

## Miten käytetään

Ehto tutkitaan vain kerran. Sijoita sanan `condition` tilalle  Boolean -lauseke, joka saa joko arvon `True` tai `False`. 

Jos totuusarvo on `True`, niin `if` ehdon komennot suoritetaan.

## Esimerkki

`if` haaran komennot suoritetaan , jos painokytkintä on painettu ja robotti pysähtyy.

```cpp
if (BumperA.pressing()) {
    Motor1.stop();
}
```

<advanced>
</advanced>