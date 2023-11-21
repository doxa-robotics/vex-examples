category: looks  
signature: brain.screen.clear_screen()  
description: Clears the entire IQ Brain's screen  

# Clear Screen

Clears the entire VEX IQ Brain's Screen.

```python
brain.screen.clear_screen()
```

## How To Use

`Clear Screen` will not reset the Brain's screen cursor. 

Use the `Set Cursor` command to set the Brain's cursor to the desired position.

## Example

This example will print "Hello", wait one second, and then clear the entire screen before printing "Goodbye".

```python
brain.screen.print("Hello")
wait(1, SECONDS)
brain.screen.clear_screen()
brain.screen.print("Goodbye")
```

<advanced>
</advanced>