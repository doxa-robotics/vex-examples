category: looks  
signature: TouchLED.brightness();  
device_class: led  
description: Sets the brightness of the touchLED.  

# Aseta KosketusLED valovoima

Asttaa VEX IQ KosketusLED :n valovoiman (valon kirkkauden).

```cpp
TouchLED.setBrightness(brightness);
```

## Miten käytetään

`TouchLED.setBrightness` hyväksyy arvot välillä **0 - 100** 'brightness` parametrille.

Komennon ensimmäinen osa on laitteen nimiesiintymä. 

```cpp
TouchLED1.setBrightness(100);
TouchLED2.setBrightness(50);
```

## Esimerkki

Tässä KosketusLED :n vihreävalo loistaa kirkkausarvolla 25 %.

```cpp
TouchLED.setBrightness(25);
TouchLED.setColor(green);
```

<advanced>
</advanced>