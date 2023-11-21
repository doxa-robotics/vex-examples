category: looks  
signature: Brain.Screen.print("Hello");  
description: Prints values or text on the V5 Brain's screen.  

# Tulosta

Tulostaa arvoja tai tekstiä V5 Aivojen näytölle.

```cpp
Brain.Screen.print("Hello World");
```

## Miten käytetään

Komento `Brain.Screen.print();` tulostaa dataa kursorin kohdalle näyttöä.

Kaikkien ohjelmien alussa paikka on rivi 1 sarake 1.

## Tulostus arvot

Voit käyttää muotoilumerkkejä print komennossasi:

* `%d` - Etumerkillinen desimaaliluku
* `%f` - Liukuluku 
* `%o` - Etumerkillinen oktaaliluku
* `%s` - Merkkijono
* `%x` - Etumerkitön hexadesimaaliluku
* `%c` - Merkki

```cpp
Brain.Screen.print("Time Elapsed %f", Brain.Timer.value());
```

Tulostettaessa voi määritellä myös desimaalien määrän. Piin koko arvo `3.14159265` voidaan kirjoittaa muodossa`3.14` kun käytät muotoilua `%.2f`.

Lukumäärä ennen desimaalia muotoilussa monellako merkillä tulostetaan. Jos tulostus on lyhyempi kuin muotoilu edellyttää, niin puuttuvat merkit täytetään tyhjillä.

Muotoilulauseke voi sisältää myös lippuja, leveyden , tarkkuuden ja alimuotoiluja:

* `%d`	- Tulostaa desimaaliluvun
* `%6d`	- Tulostaa desimaaliluvun maksimissaan 6 merkkiä leveä
* `%f`	- Tulostaa liukuluvun
* `%6f`	- Tulostaa liukuluvun maksimissaan 6 merkkiä leveä
* `%.2f`  - Tulostaa liukuluvun 2 desimaalilla
* `%6.2f` - Tulostaa liukuluvun vähintään 6 merkkiä leveä ja kahdella desimaalilla

```cpp
Brain.Screen.print("Time Elapsed %8.2f", Brain.Timer.value());
```

<advanced>
</advanced>