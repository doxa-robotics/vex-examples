category: sensing  
signature: sensing_brain_screen_row
description: Reports the row number of the Brain screen cursor location.

# Screen Cursor Row

Reports the row number of the VEX IQ Brain's screen cursor location.

```cpp
Brain.Screen.row()
```

## How To Use

### IQ (1st generation) Brain

`Brain.Screen.row` reports an integer which ranges from **1 to 5** when used with an IQ (1st generation) Brain.

### IQ (2nd generation) Brain

The IQ (2nd generation) Brain allows you to change the size of the font printed on the screen. Changing the font will affect the number of rows and columns available on the Brain's screen.

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

The `Brain.Screen.row` command reports an integer which ranges from **1 to 9** when used with an IQ (2nd generation) Brain, depending on what font is currently selected.

The value reported by `Brain.Screen.row` increases from top-to-bottom on the VEX IQ Brain's screen cursor location.

<advanced>
</advanced>