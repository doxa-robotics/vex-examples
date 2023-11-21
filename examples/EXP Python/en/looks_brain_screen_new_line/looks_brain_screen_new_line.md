category: looks  
signature: brain.screen.new_line()  
description: Sets the print output cursor on the EXP Brain's screen to the next available row.  

# Next Row

Sets the print output cursor on the EXP Brain's screen to the next available row.

```don
brain.screen.next_row()
```

## How To Use

By default, all projects begin with the screen cursor at row 1 column 1. The `brain.screen.next_row()` command will move the cursor down by a single row on the screen. `brain.screen.next_row()` will also set the cursor's column to position 1.

The EXP Brain allows you to change the size of the font printed on the screen. Changing the font will affect the number of rows available on the EXP Brain's screen.

**EXP Brain Font Size - Number of Rows:**

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
