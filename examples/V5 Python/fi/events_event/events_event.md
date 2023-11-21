category: events  
signature: EVENT(callback);
description: Broadcast event message to run listener functions.<br /><br />A user defined event will need to replace the "EVENT" in this command.<br /><br />See the help listing for broadcast() for more information.  

# Tapahtuma rekistöröi callback funtion

Rekistöröi callback -function käynnistyksen kun käyttäjätapahtuma on annettu.

```python
event(callback)
```

## Miten käytetään

Rekisteröi callback -funktio nimettyyn käyttäjätapahtumaan.

```python
def run_on_broadcast():
    brain.screen.set_cursor(1, 1)
    brain.screen.print("my_event triggered run_on_broadcast callback")
  
# Create a new event.
my_event = Event()

# Register a callback function to the myEvent event.
# Wait to allow events to register
my_event(run_on_broadcast)
wait(15, MSEC)

# Broadcast the event.
my_event.broadcast()
```

<advanced>
</advanced>