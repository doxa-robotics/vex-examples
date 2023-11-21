category: events  
signature: brain.screen.pressed(callback)  
description: Runs the callback function when the V5 Brainâ€™s touchscreen is pressed.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

#  Aivojen näyttöä koskettu

Suorittaa ns callback funktion, kun aivojen kosketusnäyttöä on kosketettu.

```python
brain.screen.pressed(callback)
```

## Miten käytetään

'brain.screen.pressed()` komennon avulla voi laukaista toimintoja, kun näyttöä on kosketettu. 

Yhdessä komennon `brain.screen.x_position()` ja `brain.screen.y_position()` kanssa saadaan interaktiivisuutta robotin ja käyttäjän välille.

Ensiksi pitää luoda funktio sille, kun näyttöä kosketetaan ja sille nimi , jota käytetään callback-funtiossa parametrina, kun tapahtuma aktivoituu.

```python
# Function to run when the event occurs
def run_on_event():
    brain.screen.print("Event has occurred")
  
# Register event with a callback function
brain.screen.pressed(run_on_event)

```

<advanced>
</advanced>