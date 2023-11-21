category: looks  
signature: touchLED.color();  
device_class: led  
description: Sets the color of the touchLED.  

# Aseta KosketusLED väri

Asettaa KosketusLED:n värin

```cpp
TouchLED.setColor(color);
```

## Miten käytetään

Komennon ensimmäinen osa on laitteen nimi.

```cpp
TouchLED1.setColor(red);
TouchLED2.setColor(green);
```
Valitse väri, jonka haluat LED :ssä näyttää.  

Väri optiot:

- `red` (punainen)
- `green` (vihreä)
- `blue` (sininen)
- `white` (valkoinen)
- `yellow` (keltainen)
- `orange` (oranssi)
- `purple` (purppura)
- `red_violet` (punavioletti)
- `violet` (violetti)
- `blue_violet` (sinivioletti)
- `blue_green` (sinivihreä)
- `yellow_green` (keltavihreä)
- `yellow_orange` (keltaoranssi)
- `red_orange` (punaoranssi)

Jos haluat kääntää KosketusLED :n valon pois päältä, aseta väri arvoon **colorType::none**.

```cpp
TouchLED.setColor(colorType::none);
```

<advanced>
</advanced>