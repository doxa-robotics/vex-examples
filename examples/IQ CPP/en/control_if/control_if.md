category: control  
signature: control_if
description: Runs the code inside the if-statement's curly brackets, if the condition returns true. 

# If

Runs the code inside if-statement's curly brackets, if the condition returns true. 

```cpp
if (condition) {
  // code to run if condition is true 
}
```

## How To Use

The **if-statement** will only check its condition inside the parentheses once.

If the condition returns **true**, the code inside the curly brackets will run.

If the condition returns **false**, the code inside the curly brackets will be skipped.

```cpp
// Stop Motor1 if BumperA is pressed
if (BumperA.pressing()) {
  Motor1.stop();
}
```

<advanced>
</advanced>