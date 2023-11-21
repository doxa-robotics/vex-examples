category: events  
signature: brain.screen.released(callback)  
description: Runs the callback function when the V5 Brainâ€™s touchscreen is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

#  Aivojen näyttöä vapautettu

Suorittaa ns callback funktion, kun aivojen kosketusnäyttöä on kosketus vapautetaan.

```python
brain.screen.released(callback)
```

## Miten käytetään

`brain.screen.released()` komennon avulla voi laukaista toimintoja näytön kosketuksen vapauttamisessa. 

Yhdessä komennon `brain.screen.x_position()` ja `brain.screen.y_position()` kanssa saadaan interaktiivisuutta robotin ja käyttäjän välille.
Ensiksi pitää luoda funktio sille, kun näyttöä kosketus loppuu ja nimi , jota käytetään callback-funtiossa parametrina , kun tapahtuma aktivoituu.

```python
# Function to run when the event occurs
def run_on_event():
    brain.screen.print("Event has occurred")
  
# Register event with a callback function
brain.screen.released(run_on_event)
```

<advanced>
</advanced>