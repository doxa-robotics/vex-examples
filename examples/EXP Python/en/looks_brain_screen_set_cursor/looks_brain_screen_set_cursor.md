category: looks  
signature: brain.screen.set_cursor(1, 1)
description: Sets the cursor location for brain.screen.print() command on the EXP Brain's screen.

# Set Cursor


Sets the cursor location on the EXP Brain's screen.

```don
brain.screen.set_cursor(ROW, COLUMN)
```

## How To Use

The `brain.screen.set_cursor()` command requires 2 values:

* Value 1: Screen row position 
* Value 2: Screen column position

Set the cursor's row and column position to have a `brain.screen.print()` command display at a specific location on the screen.

Accepts a range for **row** of **1 to 20**.

Accepts a range for **column** of **1 to 80**.


The EXP Brain allows you to change the size of the font printed on the screen. Changing the font will affect the number of rows and columns available on the EXP Brain's screen.

**EXP Brain Font Size - Number of Columns and Rows:**

| Font |  | Rows |  | Columns |
| :--- | --- | :--- | --- | :--- |
| Mono Extra Small (mono12) |  | 9 |  | 26 |
| Mono Small (mono15) |  | 7 |  | 20 |
| Mono Medium (mono20) (Default) |  | 5 |  | 16 |
| Mono Large (mono30) |  | 3 |  | 10 |
| Mono Extra Large (mono40) |  | 3 |  | 8 |
| Mono Super Large (mono60) |  | 1 |  | 5 |
| Prop Medium (prop20) |  | 5 |  | 28 |
| Prop Large (prop30) |  | 3 |  | 21 |
| Prop Extra Large (prop40) |  | 2 |  | 15 |
| Prop Super Large (prop60) |  | 1 |  | 9 |

![brain_screen_info](exp_row_column_brain.jpg)

<advanced>
</advanced>
