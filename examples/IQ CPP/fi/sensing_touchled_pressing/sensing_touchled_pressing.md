category: sensing  
signature: TouchLED.pressing()  
device_class: TouchLED
description: Reports if the VEX IQ Touch LED is pressed. 

# KosketusLED Painettu

Raportoi, jos VEX IQ KosketusLED nappia on painettu.

```cpp
TouchLED.pressing()
```

## Miten käytetään

Antaa arvon **tosi**, jos valittua KosketusLED on painettu ja arvon **epätosi**, jos lediä ei ole painettu.

Ensimmäinen osa komentoa on valittu laite-esiintymä. 

```cpp
TouchLED2.pressing()
TouchLED4.pressing()
```

## Esimerkki

Esimerkissä KosketusLED valo muutetaan arvoon **punainen**. Heti kun KosketusLediä painetaan, väri muutetaan arvoon **vihreä**.

```cpp
TouchLED.setColor(red);

while (!TouchLED.pressing()) {
  wait(20, msec);
}

TouchLED.setColor(green);
```

<advanced>
</advanced>