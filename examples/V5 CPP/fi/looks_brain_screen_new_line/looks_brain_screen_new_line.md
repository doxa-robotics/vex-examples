category: looks  
signature: Brain.Screen.newLine();  
description: Sets the print output cursor on the V5 Brain's screen to the next available row.  

# Aivojen näytölle uusi rivi

Siirtää näytöllä kursoria seuraavalle riville.

```cpp
Brain.Screen.newLine();
```

## Miten käytetään

Oletuksena aina kursori on ensimmäisen rivin ensimmäisessä sarakkeessa. Komento `Brain.Screen.newLine();` siirtää kursoria yhden rivin alemmaksi. Komento `Brain.Screen.newLine();` asetaa aina kursorin ensimmäiseen sarakkeeseen.

---

V5 Aivoille tulostettaessa voit valita kirjaisinlajin ja koon. Valinnat vaikuttavat, kuinka monta riviä ja saraketta näytölle mahtuu seuraavasti:


**V5 Brain Font Size - Number of Rows:**

* `mono12` - 20 riviä
* `mono15` - 16 riviä
* `mono20` / `prop20` - 12 riviä (Oletus)
* `mono30` / `prop30` - 8 riviä
* `mono40` / `prop40`  - 6 riviä
* `mono60` / `prop60`  - 6 riviä

![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>