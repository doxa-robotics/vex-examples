category: looks  
signature: Color.setLight(50, percent);  
device_class: Color Sensor  
description: Sets the brightness of the VEX IQ Color Sensor's light.  

# Aseta Värisensorin valon voimakkuus.

Asettaa VEX IQ Värisensorin valkoisen valon voimakkuuden. 

```cpp
Color.setLight(brightness, percent);
```

## Miten käytetään

VäriSensoria voi käyttää taskulampun tavoin valolähteenä, kun se valaisee esineitä tai pintoja paremmin.

`Color.setLight` hyväksyy parametrin arvovälin **0 - 100** valon voimakkuudelle.

Mitä isompi arvo, sitä kirkkaampi valo.

## Esimerkki

Esimerkissä Värisensorin valon voimakkuuss asetetaan arvoon 75 %.

```cpp
Color.setLight(75, percent);
```

<advanced>
</advanced>
