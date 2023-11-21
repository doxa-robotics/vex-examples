category: sensing  
signature: brain.screen.column()  
description: Reports the column number of the Brain screen cursor location  

# Screen Cursor Column

Reports the column number of the VEX IQ Brain's screen cursor location.

```python
brain.screen.column()
```

## How To Use

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

A value ranging from **1 to 28** is reported, depending on what font is currently selected.

The value of `Screen Cursor Column` increases from left-to-right on the VEX IQ Brain's screen.

<advanced>
</advanced>