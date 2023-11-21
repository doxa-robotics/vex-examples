category: sensing  
signature: Brain.Screen.xPosition()  
description: Reports the X coordinate of the location of the last detected touch on the V5 Brain's touchscreen.

# Aivojen näytön x Arvo

Antaa X-koordinaatin, johon viimeksi koskettu V5 Aivojen kosketusnäytössä.

```cpp
Brain.Screen.xPosition()
```

## Miten käytetään

`brain.screen.x_position()` kaappaa viimeisimmän näytön kosketuksen x -koordinaatin. 

Yhdessä komennon  `brain.screen.y_position()` saa molemmat koordinaatit (x,y), jolloin interaktiivisuutta voi lisätä käyttäjän ja V5 aivojen välillä.

`brain.screen.x_position()` palauttaa **integer** kokonaisluvun väliltä **0 - 480 pixeliä**.


![v5_row_column_brain](v5_row_column_brain.jpg)

```cpp
int myXCoordinate = Brain.Screen.xPosition();
```


<advanced>
</advanced>
