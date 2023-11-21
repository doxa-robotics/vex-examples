category: sensing  
signature: Motor.position(units)  
device_class: motor  
description: Reports the current position of the Motor

# Moottorin asento 

Antaa tämän hetkisen VEX IQ älymoottorin kierroslaskimen/encoderin pyörimisarvon.

```cpp
Motor.position(units)
```

## Miten käytetään

`Motor.position` palauttaa moottorin tämänhetkisen pyörimismäärän desimaalilukuna (*double*).

Valitse 'yksikkö` parametriarvoksi joko **asteita** tai **kierroksia**.

Arvot voivat olla **asteita**.

```cpp
Brain.Screen.print("Motor Position (Degrees): %.2f", Motor.position(degrees));
```

Arvot voivat olla kierroksia **turns**.

```cpp
Brain.Screen.print("Motor Position (Turns): %.2f", Motor.position(turns));
```

<advanced>
</advanced> 