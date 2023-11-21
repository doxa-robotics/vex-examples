category: looks  
signature: brain.screen.print("VEXcode")  
description: Prints values or text on the EXP Brain's screen.  

# Print

Prints values or text on the EXP Brain's screen.

```don
brain.screen.print("VEXcode")
```

## How To Use

The `brain.screen.print()` command will print data at a cursor location on the screen.

All new projects begin with the screen cursor at row 1 column 1.

* Print words and numbers: 
`brain.screen.print("Number:", 10)`

* Print the reported value from a variable: 
`brain.screen.print(my_variable)`

* Print the reported value from a sensor or device:  
`brain.screen.print(drivetrain.is_done())`

The `precision` argument is optional and specifies how many places after the decimal will be printed. The exampl,e below will print `3.14` to the Brain's screen

`brain.screen.print(3.1415926, precision=2)`

<advanced>
</advanced>
