category: control  
signature: else { }  
description: Runs the code inside the else-statement's curly brackets, if the if-statement's condition is false. This command must have an if-statement preceding for it to compile.  

# If/Else

Runs the code inside the else-statement's curly brackets, if the if-statement's condition is false. This command must have an if-statement preceding for it to compile.

```cpp
if (condition) {

} else {

}
```

## How To Use

The **if-statement** will only check its condition inside the parenthesis once.

If the condition returns **true**, the code inside the if-statement's curly brackets will run.

If the condition returns **false**, the code inside the else-statement's curly brackets will be skipped

```cpp
if (BumperA.pressing()) {
    LeftMotor.stop();
} else {
    LeftMotor.spin(forward);
}
```

<advanced>
</advanced>