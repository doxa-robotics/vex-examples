category: events  
signature: EVENT.broadcastAndWait();    
description: Broadcast event message to run listener functions and wait for all listeners to finish before continuing.<br /><br />A user defined event will need to replace the "EVENT" in this command.<br /><br />See the help listing for broadcastAndWait() for more information.  

# Event Broadcast and Wait

Broadcast event message to run listener functions and wait for all listeners to finish before continuing.

```cpp
Event.broadcastAndWait();
```

## How To Use

The `Event.broadcastAndWait();` command will wait for all listeners to complete before returning. This will pause the code execution in the current function, until all the broadcast listeners have finished.

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

  // Broadcast the event and wait for completion.
  myEvent.broadcastAndWait();

  Brain.Screen.setCursor(3, 1);
  Brain.Screen.print("Listeners finished running");
}
```

<advanced>
</advanced>