category: looks  
signature: controller.screen.print("VEXcode")  
description: Prints values or text on the V5 Controller's screen.  

# Print  

Prints values on the V5 Controller's screen.

```don
controller.screen.print("VEXcode") 
```

## How To Use

The `controller.screen.print()` command will print data at a cursor location on the screen.

All new projects begin with the screen cursor at row 1 column 1.

* Print words and numbers: 
`controller.screen.print("Number:", 10)`

* Print the reported value from a variable:  
`controller.screen.print(my_variable)`

* Print the reported value from a sensor or device: 
`controller.screen.print(drivetrain.is_done())`
	
<advanced>
</advanced>
