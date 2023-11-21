category: looks  
signature: Brain.Screen.drawLine(1, 1, 10, 10);  
description: Draws a line on the V5 Brain's screen.  

# Piirrä viiva

Piirtää viivan V5 aivojen näytölle.
```cpp
Brain.Screen.drawLine(1, 1, 10, 10);
```

## Miten käytetään

`Brain.Screen.drawLine();` komeNto vaatii 4 arvoa:

* Arvo 1: Alkupiste X koordinaatti
* Arvo 2: Alkupiste Y koordinaatti
* Arvo 3: Loppupiste X koordinaatti
* Arvo 4: Loppupiste Y koordinaatti

Viivan väri määrätään komennolla `Brain.Screen.setPenColor();`. Oletuksena on valkoinen viiva.

![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>