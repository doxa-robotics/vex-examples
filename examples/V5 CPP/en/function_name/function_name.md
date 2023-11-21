category: functions  
signature: function_name
device_class: function  
description: Runs the specified function when the bumper is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Functions

Functions are segments of code used to perform a set of actions.

```cpp
void myFunction() {
  // function code
}
```

## How To Use

To define a function, declare the type of data that the function will return.

- `int`, `float`, `double`, and `string` are commonly returned data types. If the function will not return a value declare the return type as `void`. 

Then, use a meaningful function name that describes what the function does.

```cpp
int returnZero() {
  return 0;
}
```

Include parentheses `()` with optional *parameters* after the function name. Multiple parameters should be separated by commas (parameter1, parameter2).

The body of the function should be enclosed in curly brackets `{ }`.
    
## Example

This function has no parameters and returns no value and so its return type is declared as `void`. This function prints "The battery is low!" to the VEX V5 Brain Screen if the battery capacity is below 25%.

```cpp
void lowOnBattery() {
  if (Brain.Battery.capacity() < 25.0) {
    Brain.Screen.print("The battery is low!");
  }
}
```

<advanced>
</advanced>