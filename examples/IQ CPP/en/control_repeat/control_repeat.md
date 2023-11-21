category: control  
signature: repeat(10) { }  
description: Repeats the code inside curly brackets for a set number of times.

# Repeat

Repeats the commands inside curly brackets for the number set inside the parentheses.
`repeat (number of times to repeat){code to repeat}`

```
repeat (10) {

}
```

## How To Use

The **repeat-statement** will loop through the code contained in the brackets until it reaches the number of iterations set in the condition.

First, set the number of times the code will loop by changing the condition to any positive integer. The condition can also be a variable or sensor data.

The snippet below will print "iteration" to the Brain's Screen four times. Each time, it will create a new line before printing the next iteration.

```
repeat (4) {
  Brain.Screen.print("iteration");
  Brain.Screen.newLine();
  wait(5, msec);
}
```

Note that the **repeat-statement** cannot be nested inside of another repeat statement.

<advanced>
</advanced>