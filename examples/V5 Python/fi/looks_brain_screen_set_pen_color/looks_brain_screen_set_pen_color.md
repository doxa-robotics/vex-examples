category: looks  
signature: brain.screen.set_pen_color(Color.RED)  
description: Sets the color of lines drawn on the V5 Brain's screen.  

# Aseta kynän väri

Asettaa kynän värin V5 Aivojen näytölle piirrettäessä.

```don
brain.screen.set_pen_color(COLOR)
```

## Miten käytetään

Komentoa `brain.screen.set_pen_color()` käytetään, kun kynän väri valitaa piirrettäessä viivoja, pixeleitä tai tekstiä V5 näytölle. 

`brain.screen.set_pen_color()` sopii myös neliöiden ja monikolmioiden ääriviivojen piirtoon.

Valise joku seuraavista väreistä:

* `Color.BLACK`
* `Color.WHITE`
* `Color.RED`
* `Color.GREEN`
* `Color.BLUE`
* `Color.YELLOW`
* `Color.ORANGE`
* `Color.PURPLE`
* `Color.CYAN`

Kynäväri säilyy kunnes otat käyttöön uuden värin.
<advanced>
</advanced>
