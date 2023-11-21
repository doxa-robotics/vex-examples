category: looks  
signature: brain.screen.new_line()  
description: Sets the print output cursor of the Print Console to the next line.  

# Next Row

Sets the print output cursor of the Print Console to the next line.

```don
brain.screen.next_row()
```

## How To Use

By default, all projects begin with the print cursor at row 1. The `brain.screen.next_row()` command will move the cursor down by a single line on the Print Console.

---

```python
# Print "VEXcode" on the first line, then "V5" on the next line
brain.screen.print("VEXcode")
brain.screen.next_row()
brain.screen.print("V5")
```

<advanced>
</advanced>
