category: looks  
signature: brain.screen.print("VEXcode")  
description: Prints values or text to the Print Console.  

# Print

Prints values or text to the Print Console.

```don
brain.screen.print("VEXcode")
```

## How To Use

The `brain.screen.print()` command will print data to the Print Console.

* Print words and numbers: 
`brain.screen.print("Number:", 10)`

* Print numbers with decimal points:
```brain.screen.print("Timer Value:", brain.timer.time(SECONDS), precision=2)```

* Print the reported value from a variable: 
`brain.screen.print(my_variable)`

* Print the reported value from a sensor or device:  
`brain.screen.print(drivetrain.is_done())`

<advanced>
</advanced>
