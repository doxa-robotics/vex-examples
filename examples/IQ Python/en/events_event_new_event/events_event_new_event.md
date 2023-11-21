category: events  
signature: my_event = Event() 
description: Create a new user-defined event.  

# New Event

Create a new event.

```python
my_event = Event()
```

## How To Use

Using the above syntax, a new user-defined event can be created before registering callback functions.

```python
def run_on_broadcast1():
    brain.screen.set_cursor(1, 1)
    brain.screen.print("Broadcast1")

def run_on_broadcast2():
    brain.screen.set_cursor(2, 1)
    brain.screen.print("Broadcast2")

# Create new events.
my_event1 = Event()
my_event2 = Event()

# Register callback functions to the events.
# Wait to allow events to register
my_event1(run_on_broadcast1)
my_event2(run_on_broadcast2)
wait(15, MSEC)

# Broadcast the events.
my_event1.broadcast()
my_event2.broadcast()
```

<advanced>
</advanced>