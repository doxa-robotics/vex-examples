category: events  
signature: limit.released(callback)  
device_class: limit  
description: Runs the specified function when the Limit Switch is released.  

# Limit Switch vapautettu

Suoritetaan määritelty funktio kun Limit Switch vapautettu.
```python
limit.released(callback)
```

## Miten käytetään

Sensorin painallusta varten pitää määritellä funktio , jota kutsutaan vapautuksen jälkeen. 

Anna funktiolle nimi ja määrittele sen toiminta, kun tapahtuma Limit Switch vapautettu . Kyseessä on ns `callback` parametri tapahtumalle.

```python
# Function to run when the event occurs
def run_on_limit_released():
    brain.screen.print("Limit released!")
 
# Register event with a callback function
limit_a.released(run_on_limit_released)
`

<advanced>
</advanced>