category: events  
signature: EVENT.broadcast();  
description: Broadcast event message to run listener functions.<br /><br />A user defined event will need to replace the "EVENT" in this command.<br /><br />See the help listing for broadcast() for more information.  

# Event Broadcast

Broadcast event message to run listener functions.

```cpp
Event.broadcast();
```

## How To Use

The code will continue to run the commands after the `Event.broadcast();` command so that it will run at the same time as the event listener functions.

Before using this command, a user defined event must be created and register at least one callback.

```cpp
void runOnBroadcast1() {
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Broadcast1 Running");
}

void runOnBroadcast2() {
  Brain.Screen.setCursor(2, 1);
  Brain.Screen.print("Broadcast2 Running");
}

int main() {
  // Create a new event.
  event myEvent;

  // Register callback functions to event.
  myEvent(runOnBroadcast1);
  myEvent(runOnBroadcast2);
  
  // Brief wait to ensure event is registered
  wait(15, msec);

  // Broadcast the event.
  myEvent.broadcast();
}
```

<advanced>
</advanced>