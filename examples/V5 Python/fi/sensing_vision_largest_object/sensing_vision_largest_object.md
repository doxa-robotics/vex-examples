category: sensing  
signature: vision.largest_object()
description: Reports information about the largest detected object from the Vision Sensor.

# Suurin esine

Antaa tiedot suurimmasta Vision kameran havaitusta esineestä.

```python
vision.largest_object()
```

## Miten käytetään

Määrittele Vision kamera lisäämällä esineiden merkit/koodit.

Tee `vision.take_snapshot` komento ottamaan kuva ja käytä `vision.largest_object` komentoa.

Esimerkissä tulsottetaan näytölle tietoja havaitusta esineestä.

```python
while True:
    brain.screen.clear_screen()
    brain.screen.set_cursor(1, 1)

    # Take a snapshot with the Vision Sensor with the specified signature and store the object data into a variable
    vision_object = vision.take_snapshot(signature)

    # Check the variable to see if a valid object was detected when the snapshot was captured
    # If yes, print the data
    if vision_object is not None:
        brain.screen.print("Center X: ", vision.largest_object().centerX)
        brain.screen.next_row()

        brain.screen.print("Center Y: ", vision.largest_object().centerY)
        brain.screen.next_row()

        # Take a new snapshot every 0.2 seconds
        wait(0.2, SECONDS)
    else:
        brain.screen.print("No Object Detected")
```

Seuraavassa listta ominaisuuksista, joita voi käyttää `vision.largest_object` komennon jälkeen:

- `id` - Yksikäsitteinen ID jokaiselle Vision kamera objektille
- `originX` - Ylä vasen X arvo esineestä
- `originY` - Ylä vasen Y arvo esineestä
- `centerX` - Keskipiste X arvo esineestä
- `centerY` - Keskipiste Y arvo esineestä
- `width` - Esineen leveys
- `height` - Esineen korkeus
- `angle` - Esineen kulma kameraan
- `exists` - Havaitseeko Vision kamera esineen

<advanced>
</advanced>
