category: events  
signature: my_event.broadcast()  
description: Broadcast event message to run listener functions.<br /><br />A user defined event will need to replace the "EVENT" in this command.<br /><br />See the help listing for broadcast() for more information.  

# Tapahtuman lähetys

Lähettää tapahtumaviestin käynnistää vastaavan tapahtumafunktion.

```python
event.broadcast()
```

## Miten käytetään

Ohjelma jatkaa suoritusta samaan aikaan kun `event.broadcast()` komentoa suoritetaan kutsutun callback-funtion osalta.

Ennen kutsun käyttöä pitää tapahtuma olla määritelty ja rekistöröidä vastaava vähintää yksi callback-funtio.

```python
def run_on_broadcast1():
    brain.screen.set_cursor(1, 1)
    brain.screen.print("Broadcast1 Running")

def run_on_broadcast2():
    brain.screen.set_cursor(2, 1)
    brain.screen.print("Broadcast2 Running")
  
# Create a new event.
my_event = Event()

# Register callback functions to event.
# Wait to allow events to register
my_event(run_on_broadcast1)
my_event(run_on_broadcast2)
wait(15, MSEC)

# Broadcast the event.
my_event.broadcast()

```

<advanced>
</advanced>