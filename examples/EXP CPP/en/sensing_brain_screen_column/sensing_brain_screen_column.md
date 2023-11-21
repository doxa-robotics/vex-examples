category: sensing  
signature: Brain.Screen.column()  
description: Reports the column number of the EXP Brain screen cursor location.

# Brain Screen Column
Reports the column number of the EXP Brain screen cursor location.

```cpp
Brain.Screen.column()
```

## How To Use

The EXP Brain allows you to change the size of the font printed on the screen. Changing the font will affect the number of rows and columns available on the Brain's screen.

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

A value ranging from **1 to 28** is reported if used with an EXP Brain, depending on what font is currently selected.

The value of `Brain.Screen.column` increases from left-to-right on the EXP Brain's screen.

![brain_screen_info](exp_row_column_brain.jpg)

<advanced>
</advanced>