category: control  
signature: if(true) { }  
description: Runs the code inside the if-statement's curly brackets, if the condition returns true. 

# If

Runs the code inside if-statement's curly brackets, if the condition returns true. 

```cpp
if (condition) {

}
```

## How To Use

The **if-statement** will only check its condition inside the parenthesis once.

If the condition returns **true**, the codes inside the curly brackets will run.

If the condition returns **false**, the codes inside the curly brackets will be skipped.

```cpp
if (BumperA.pressing()) {
    Motor1.stop();
}
```

<advanced>
</advanced>