category: events  
signature: Brain.Timer.event(callback, 1000);  
description: Runs the specified function when the Brain's timer is greater than the given value.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Brain Timer Event

Sets a callback that will be called after the specified amount of time.

```cpp
Brain.Timer.event(callback, time);
```

## How To Use

The EXP Brain's timer begins at the start of each program.

The `Brain.Timer.event` function takes 2 parameters.

The first is the **callback function** parameter. A function will need to be created to pass to the `Brain.Timer.event` function.

The second parameter is the time at which the function will run. The **callback function** will run once the **Brain Timer** is greater than the entered amount. The amount of `time` should be in **milliseconds**.

```cpp
// Call the callback function after 1000 milliseconds
Brain.Timer.event(callback, 1000);
```

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs.

In the snippet below, "Callback Function Called" will be printed to the Brain Screen after 10 seconds.

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Brain.Timer.event(callbackFunction, 10000);
}
```


<advanced>
</advanced>