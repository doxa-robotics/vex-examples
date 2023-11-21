category: sensing  
signature: Brain.Screen.column()  
description: Reports the column number of the V5 Brain screen cursor location.

# Aivojen näytön kursorin sarake
ANtaa sarakenumeron, jolla kursori tällä hetekllä aivojen näytöllä.

```cpp
Brain.Screen.column()
```

```cpp
if (Brain.Screen.column() > 10.0) {
  Brain.Screen.print("Cursor is past column 10");
}
```
---

## Miten käytetään

Näytön sarake voi olla välillä **1 - 80**.

```cpp
if (Brain.Screen.column() > 10.0) {
  Brain.Screen.print("Cursor is past column 10");
}
```
---

V5 Aivojen näytöklle voi määritellä fontin kokoa ja samaal se vaikuttaa sarakkeiden määrään.

**V5 Aivojen fonttikokoe - Sarakkeiden määrä:**

* `FontType.MONO12` - 80 saraketta
* `FontType.MONO15` - 68 saraketta
* `FontType.MONO20` / `FontType.PROP20` - 48 saraketta (Oletus)
* `FontType.MONO30` / `FontType.PROP30` - 32 saraketta
* `FontType.MONO40` / `FontType.PROP40` - 24 saraketta
* `FontType.MONO60` / `FontType.MONO60` - 16 saraketta
* 
![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>