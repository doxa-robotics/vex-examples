category: events  
signature: optical.object_lost(callback)   
device_class: optical  
description: Runs the callback function when an object is no longer being detected by a V5 Optical Sensor  

# Optical kohde hävisi

Ajetaan callback funktio, kun V5 Optical Sensori kadottaa äskeisen esineen.

```python
optical.object_lost(callback)
```

## Miten käytetään

`optical.object_lost` komento käynnistää halutut toimenpiteet, kun V5 Optical sensori ei enää havaitse kohdetta/esinettä.

Luo funktio, jota kutsutaan kun esinettä ei enää havaita. Anna funktiolle nimi , joka kutsutaan, kun tapahtuma ilmenee **callback** parametrissa.

```python
# Function to run when the event occurs
def run_on_object_lost():
    brain.screen.print("Object lost!")

# Register an event with a callback function
optical.object_lost(run_on_object_lost)
```

<advanced>
</advanced>







