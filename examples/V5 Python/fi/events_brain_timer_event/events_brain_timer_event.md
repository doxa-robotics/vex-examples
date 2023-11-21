category: events  
signature: brain.timer.event(callback, 1000)
description: Runs the specified function when the V5 Brain's timer is greater than the given value.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Aivojen kello tapahtuma

Suorittaa halutun callback funktion, kun V5 Aivojen kello on suurempi kuin annettu parametriarvo.

```python
brain.timer.event(callback, 1000)
```

## Miten käytetään

V5 Aivojen kello käynnistyy ohjelman alussa.

Määritä aikaraja tapahtumalle. `brain.timer.event()` tapahtuma suoritetaan kerran kun kello on **suurempi kuin** annettu aikaraja.

`brain.timer.event()` hyväskyy kokonaislukuja ja yksikkönä on millisekunnit.

Luo funktio , jota kutsutaan, kun kello käynyt yli aikarajan. Nimeä funktio ja käytä sitä tapahtuman `callback` parametrina.

```python
# Function to run when the event occurs
def run_on_event():
    brain.screen.print("Event has occurred")
  
# Register event with a callback function
brain.timer.event(run_on_event, 2000)
```


<advanced>
</advanced>