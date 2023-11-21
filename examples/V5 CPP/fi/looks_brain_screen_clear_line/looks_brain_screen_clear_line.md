category: looks  
signature: Brain.Screen.clearLine();  
description: Clears a single row on the V5 Brain screen.  

# Tyhjää rivi

Tyhjää yksittäisen rivin V5 aivojen tai ohjaimen näytöllä.


```cpp
Brain.Screen.clearLine();
```

## Miten käytetään

Tyhjää nykyisen kursoririvin.


```cpp
Brain.Screen.clearLine();
```

Tyhjää tietyn rivin 1 näytöllä.

```cpp
Brain.Screen.clearLine(1);
```

## Miten käytetään

`Brain.Screen.clearLine();` komento hyväksyy arvot välillä **1 - 20**, jonka rivin tyhjää. Ilman rivinumero komento tyhjää nykyisen rivin.


The V5 Brain allows you to change the size of the font printed on the screen. Changing the font will affect the number of lines available on the V5 Brain's screen.

**V5 Aivojen fonttikoko - rivimäärä:**

* `mono12` - 20 riviä
* `mono15` - 16 riviä
* `mono20` / `prop20` - 12 riviä (oletus)
* `mono30` / `prop30` - 8 riviä
* `mono40` / `prop40` - 6 riviä
* `mono60` / `prop60` - 4 riviä

![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>