category: events  
signature: events_event_broadcast_and_wait   
description: Broadcast event message to run listener functions and wait for all listeners to finish before continuing.

# Broadcast and Wait

Broadcasts a message to activate any functions that are passed to the **Event** while also pausing the rest of the current program.

```cpp
myEvent.broadcastAndWait();
```

## How To Use

The `myEvent.broadcastAndWait` command will wait for all listeners to complete before returning. This will pause the code execution in the current function until all the broadcast listeners have finished execution.

Before using this command, an event must be created and have at least one callback registered.

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Function Called.");

  wait(5, seconds);
}

int main() {
  // Register a new event in the main function and pass the callbackFunction
  event myEvent = event(callbackFunction);

  // Broadcast the event and wait for it to finish executing
  myEvent.broadcastAndWait();

  // This will not run until the callbackFunction has completed execution
  Brain.Screen.newLine();
  Brain.Screen.print("Done!");
}
```

<advanced>
</advanced>