category: looks  
signature: brain.screen.draw_line(1, 1, 10, 10)  
description: Draws a line on the V5 Brain's screen.  

# Piirrä viiva

Piirtää viivan V5 aivojen näytölle.

```don
brain.screen.draw_line(START_X, START_Y, END_X, END_Y)
```

## Miten käytetään

`brain.screen.draw_line()` komeNto vaatii 4 arvoa:

* Arvo 1: Alkupiste X koordinaatti
* Arvo 2: Alkupiste Y koordinaatti
* Arvo 3: Loppupiste X koordinaatti
* Arvo 4: Loppupiste Y koordinaatti

Viivan väri määrätään komennolla `brain.screen.set_pen_color()`. Oletuksena on valkoinen viiva.

![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>
