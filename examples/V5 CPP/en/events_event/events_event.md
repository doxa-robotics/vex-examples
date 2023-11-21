category: events  
signature: EVENT(callback);
description: Broadcast event message to run listener functions.<br /><br />A user defined event will need to replace the "EVENT" in this command.<br /><br />See the help listing for broadcast() for more information.  

# Event Register Callback

Register a callback function to run when an event is triggered.

```cpp
Event(callback);
```

## How To Use

Register a callback to a user-defined event.

```cpp
void runOnBroadcast() {
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("myEvent triggered runOnBroadcast callback");
}

int main() {
  // Create a new event.
  event myEvent;

  // Register a callback function to the myEvent event.
  myEvent(runOnBroadcast);
  
  // Brief wait to ensure event is registered
  wait(15, msec);

  // Broadcast the event.
  myEvent.broadcast();
}
```

<advanced>
</advanced>