category: looks  
signature: TouchLED.setFade(fade);  
device_class: led  
description: Sets the fade speed of the touchLED.

# Aseta KosketusLED värinvaihto

Asettaa värinvaihdon nopeuden, kun VEX IQ KosketusLED vaihtaa väriä.

```cpp
TouchLED.setFade(fade);
```

## Miten käytetään

Komennon ensimäinen osa on laitenimen valinta.

```cpp
TouchLED1.setFade(fast);
TouchLED2.setFade(slow);
```
Valitse värinvaihdon nopeus:

* **slow** - KosketusLED hitaasti vaihtaa toiseen väriin
* **fast** - KosketusLED nopeasti vaihtaa toiseen väriin
* **off** - KosketusLED heti vaihtaa toiseen väriin

## Esimerkki

Tässä esimerkissä vaihdetaan LED:n väriä hitaasti punaisesta siniseen.

```cpp
TouchLED.setColor(red);
TouchLED.setFade(slow);
TouchLED.setColor(blue);
```

<advanced>
</advanced>