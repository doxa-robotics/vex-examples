category: looks  
signature: Brain.Screen.drawRectangle(1, 1, 10, 10);  
description: Draws a rectangle on the V5 Brain's screen.  

# Piirrä suorakulmio

Piirtää suorakulmion V5 Aivojen näytölle.

```cpp
Brain.Screen.drawRectangle(1, 1, 10, 10);
```

## Miten käytetään

Komento `Brain.Screen.drawRectangle();' vaatii 4 arvoa:

* Arvo 1: Ylä vasen nurkka X koordinaatti
* Arvo 2: Ylä vasen nurkka Y koordinaatti
* Arvo 3: Leveys kulmiolle
* Arvoe 4: Korkaus kulmiolle

Komento `Brain.Screen.setPenColor();` määrää reunaviivan värin. Oletus on valkoinen.

Täyttöväri saadaan komennolla `Brain.Screen.setFillColor();`. Oletus on musta täyttöväri.

![brain_screen_info](v5_row_column_brain.jpg)


<advanced>
</advanced>