category: events  
signature: EVENT.broadcast();  
description: Broadcast event message to run listener functions.

# Broadcast

Broadcasts a message to activate any functions that are passed to the **Event**.

```cpp
myEvent.broadcast();
```

## How To Use

The code will continue to run the commands after the `myEvent.broadcast` command so that it will run at the same time as the event listener functions.

Before using this command, a user-defined event must be created and register at least one callback.

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
  // Create an event in the main function
  event myEvent = event();

  // Register callback functions to event
  myEvent(runOnBroadcast1);
  myEvent(runOnBroadcast2);

  // Broadcast the event
  myEvent.broadcast();
}
```

<advanced>
</advanced>