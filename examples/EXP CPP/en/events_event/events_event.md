category: events  
signature: EVENT(callback);
description: Broadcast event message to run listener functions.<br /><br />A user defined event will need to replace the "EVENT" in this command.<br /><br />See the help listing for broadcast() for more information.  

# Event Register Callback

Creates a new event to trigger user defined functions.

```cpp
event myEvent = event(callbackFunction);
```

## How To Use
The **event** object can be used to trigger a user defined function. To use it, an **event** object needs to be created. This can be done in two ways.

A **callback function** can be used as an argument to the creation function.

```cpp
event myEvent = event(callbackFunction);
```
A **callback function** does not need to be passed to the creation function.

```cpp
event myEvent = event();
```
Multiple **callback functions** can be added to an event. All of the functions will be called and ran at the same time when the event occurs.

```cpp
event myEvent = event();
myEvent(callbackFunction1);
myEvent(callbackFunction1);
```
Only **2 event callback functions** should run at the same time. Additional **events callback functions** may reduce the performance of the VEX EXP robot.

The callback functions will execute when either the `myEvent.broadcast` or `myEvent.broadcastAndWait` functions are called.

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Function Called.");
}

int main() {
  // Create a new event called myEvent in the main function and pass callbackFunction
  event myEvent = event(callbackFunction);

  // Broadcast myEvent, triggering "Function Called." to be printed to the Brain's Screen
  myEvent.broadcast();
}
```

<advanced>
</advanced>