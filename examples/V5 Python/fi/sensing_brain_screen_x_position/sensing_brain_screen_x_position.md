category: sensing  
signature: brain.screen.x_position() 
description: Reports the X coordinate of the location of the last detected touch on the V5 Brain's touchscreen.

# Aivojen näytön x Arvo

Antaa X-koordinaatin, johon viimeksi koskettu V5 Aivojen kosketusnäytössä.

```python
brain.screen.x_position()
```

## Miten käytetään

`brain.screen.x_position()` kaappaa viimeisimmän näytön kosketuksen x -koordinaatin. 

Yhdessä komennon  `brain.screen.y_position()` saa molemmat koordinaatit (x,y), jolloin interaktiivisuutta voi lisätä käyttäjän ja V5 aivojen välillä.

`brain.screen.x_position()` palauttaa **integer** kokonaisluvun väliltä **0 - 480 pixeliä**.

![v5_row_column_brain](v5_row_column_brain.jpg)

```python
my_x_coordinate = brain.screen.x_position()
```


<advanced>
</advanced>
