category: sensing  
signature: brain.screen.y_position()
description: Reports the Y coordinate of the location of the last detected touch on the V5 Brain's touchscreen.

# # Aivojen näytön y Arvo

Antaa Y-koordinaatin, johon viimeksi koskettu V5 Aivojen kosketusnäytössä.

```python
brain.screen.y_position()
```

## Miten käytetään

`brain.screen.y_position()` kaappaa viimeisimmän näytön kosketuksen x -koordinaatin. 

Yhdessä komennon  `brain.screen.x_position()` saa molemmat koordinaatit (x,y), jolloin interaktiivisuutta voi lisätä käyttäjän ja V5 aivojen välillä.

`brain.screen.y_position()` palauttaa **integer** kokonaisluvun väliltä **0 - 240 pixeliä**.

![v5_row_column_brain](v5_row_column_brain.jpg)

```python
my_y_coordinate = brain.screen.y_position()
```

<advanced>
</advanced>
