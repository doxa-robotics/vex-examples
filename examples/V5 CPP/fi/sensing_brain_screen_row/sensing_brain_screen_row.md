category: sensing  
signature: Brain.Screen.row()  
description: Reports the row number of the V5 Brain screen cursor location.

# Kursorin rivi aivojen näytöllä

Antaa kursorin rivinumeron V5 aivojen näytöllä.

```cpp
Brain.Screen.row()
```

## Miten käytetään

Näytön rivien lukumäärä oletusfontilla on välillä **1 to 20**.



```cpp
if (Brain.Screen.row() > 10.0) {
  Brain.Screen.print("Cursor position is past row 10");
}
```
---

Voit muuttaa fontin kokoa näytöllä ja samalla se vaikuttaa rivien määrään:

**V5 Aivojen fonttikoko - Rivien määrä:**

* `mono12` - 20 riviä
* `mono15` - 16 riviä
* `mono20` / `prop20` - 12 riviä (Oletus)
* `mono30` / `prop30` - 8 riviä
* `mono40` / `prop40` - 6 riviä
* `mono60` / `prop60` - 4 riviä

![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>