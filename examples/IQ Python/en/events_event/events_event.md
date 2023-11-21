category: events  
signature: EVENT(callback);
description: Broadcast event message to run listener functions.<br /><br />A user defined event will need to replace the "EVENT" in this command.<br /><br />See the help listing for broadcast() for more information.  

# Event Register Callback

Register a callback function to run when an event is triggered.

```python
event(callback)
```

## How To Use

Register a callback to a user-defined event.

```python
def run_on_broadcast():
    brain.screen.set_cursor(1, 1)
    brain.screen.print("my_event")
    brain.screen.next_row()
    brain.screen.print("broadcasted")
  
# Create a new event.
my_event = Event()

# Register a callback function to the my_event event
# Wait to allow events to register
my_event(run_on_broadcast)
wait(15, MSEC)

# Broadcast the event
my_event.broadcast()
```

<advanced>
</advanced>