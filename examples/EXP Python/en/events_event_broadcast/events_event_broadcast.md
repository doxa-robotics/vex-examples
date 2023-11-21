category: events  
signature: my_event.broadcast()  
description: Broadcast event message to run listener functions.<br /><br />A user defined event will need to replace the "EVENT" in this command.<br /><br />See the help listing for broadcast() for more information.  

# Event Broadcast

Broadcast event message to run listener functions.

```python
event.broadcast()
```

## How To Use

The code will continue to run the commands after the `event.broadcast()` command so that it will run at the same time as the event listener functions.

Before using this command, a user defined event must be created and register at least one callback.

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