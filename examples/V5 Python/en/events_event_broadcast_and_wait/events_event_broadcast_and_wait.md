category: events  
signature: my_event.broadcast_and_wait()    
description: Broadcast event message to run listener functions and wait for all listeners to finish before continuing.<br /><br />A user defined event will need to replace the "EVENT" in this command.<br /><br />See the help listing for broadcastAndWait() for more information.  

# Event Broadcast and Wait

Broadcast event message to run listener functions and wait for all listeners to finish before continuing.

```cpp
event.broadcast_and_wait()
```

## How To Use

The `event.broadcast_and_wait()` command will wait for all listeners to complete before returning. This will pause the code execution in the current function, until all the broadcast listeners have finished.

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

# Broadcast the event and wait for completion.
my_event.broadcast_and_wait()

brain.screen.set_cursor(3, 1)
brain.screen.print("Listeners finished running")
```

<advanced>
</advanced>