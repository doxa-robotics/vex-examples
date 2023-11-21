category: events  
signature: optical.object_detected(callback)   
device_class: optical  
description: Runs the callback function when an object is detected by a V5 Optical Sensor  

# Optical löytää esineen

Suorittaa callback funktion kun V5 Optical Sensori havaitsee esineen/kohteen.

```python
optical.object_detected(callback)
```

## Miten käytetään

`optical.object_detected` komentoa voi käyttää triggeröimään haluttuja toimintoja kun V5 Optical Sensori havaitsee kohteen/esineen.

Sinun pitää luoda funktio, joka suoritetaan kun esine havaitaan. Anna funktiolle nimi , joka annetaan **callback** parametrissa ja suoritetaan kun esine havaitaan.

```python
# Function to run when the event occurs
def run_on_object_detected():
    brain.screen.print("Object detected!")

# Register an event with a callback function
optical.object_detected(run_on_object_detected)
```

<advanced>
</advanced>







