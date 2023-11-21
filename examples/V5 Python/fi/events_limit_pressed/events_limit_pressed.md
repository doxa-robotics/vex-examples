category: events  
signature: limit.pressed(callback)  
device_class: limit  
description: Runs the specified function when the Limit Switch is pressed.  

# Limit Switch painettu

Suoritetaan määritelty funktio kun Limit Switch painettu.

```python
limit.pressed(callback)
```

## Miten käytetään

Sensorin painallusta varten pitää määritellä funktio , jota kutsutaan painalluksen jälkeen. 

Anna funktiolle nimi ja määrittele sen toiminta, kun tapahtuma Limit Switch painettu . Kyseessä on ns `callback` parametri tapahtumalle.

```python
# Function to run when the event occurs
def run_on_limit_pressed():
    brain.screen.print("Limit pressed!")
 
# Register event with a callback function
limit_a.pressed(run_on_limit_pressed)
```

<advanced>
</advanced>