category: looks  
signature: CONTROLLER.Screen.print("Hello");  
device_class: controller  
description: Prints values or text on the V5 Controller's screen.  

# Ohajimen näytölle tulostus

Tulostaa arvoja V5 ohjaimen näytölle.

```cpp
Controller.Screen.print("Hello World");
```

## Miten käytetään

`Controller.Screen.print();` komento tulostaa dataa kursorin kohdalle näytöllä.

Aina ohjelman alussa paikka on rivi 1 sarake 1.

## Printing Values

Voit käyttää format tarkennuksia tulostuksessa seuraavasti:

* `%d` - Etumerkillinen Desimaali / Kokonaisluku
* `%f` - Liukuluku
* `%o` - etumerkillinen oktaali kokonaisluku
* `%s` - Tekstijono
* `%x` - eutumerkitön hexadecimaaliluku
* `%c` - Merkki

```cpp
Controller1.Screen.print("Timer: %f", Brain.Timer.value());
```

Tulostettavat arvoille voit määrittää desimaalien määrän, arvolle  `3.14159265` voit halutessa tulostaa kahdella desimaalilla `3.14` antamalla formaattitarkennin `%.2f`.

Numero ennen desimaalia kertoo montako merkkiä haluat tulostaa, kun taas numero desimaalimerkin jälkeen kertoo monellako desimaalilla tulostetaan.

Formaattitarkennin voi sisältää myös muita tarkennuksia lippuja, leveys, tarkkuus ja alitarkentimia:

* `%d`	- Tulostaa desimaali(kokonais)luvun
* `%6d`	- Tulostaa desimaaliluvun vähintään 6 merkin leveydellä
* `%f`	- Tulostaa liukuluvun
* `%6f`	- Tulostaa liukuluvun vähintään 6 merkin leveydellä
* `%.2f`  - Tulostaa liukuluvun kahdella desimaalilla
* `%6.2f` - Tulostaa desimaaliluvun vähintään 6 merkin leveydellä kahdella desimaalilla

```cpp
Controller1.Screen.print("Timer: %8.2f", Brain.Timer.value());
```

<advanced>
</advanced>