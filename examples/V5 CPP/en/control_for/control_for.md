category: control  
signature: for(int i = 0; i < length; i++) { }  
description: A type of loop that repeats the code contained inside for a set number of iterations. 

# For

A type of loop that repeats the code contained inside for a set number of iterations.

```cpp
for (initialization; condition; increment/decrement) {
   // code here will repeat a number of times
}
```

## How To Use

First enter a value to indicate how many times the stack will **repeat** the code contained inside.

The **for** loop keeps track of how many times to repeat using 3 expressions:

* initialization
* condition
* increment/decrement expression.

**Initialization** specifies the initial value of the iterating variable. You can also declare a variable in the initialization statement.

**Condition** is used to set the condition to specify how long the **for** loop will continue running. The **for** loop will stop looping if the counter value will return false using this condition.

**Increment/decrement** expression is used to change the iterating variable at the end of each iteration of the **for** loop.

The following for-loop will print a number 0 to 9:

```cpp
for(int i = 0; i < 10; i++) {
   Brain.Screen.print(i);
   Brain.Screen.newLine();
}
```

**For** loops can also be put inside of each other. This concept is called nesting which can help save time when programming different behaviors.

<advanced>
</advanced>