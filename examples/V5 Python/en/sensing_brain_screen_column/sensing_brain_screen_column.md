category: sensing  
signature: brain.screen.column()  
description: Reports the column number of the V5 Brain screen cursor location.

# Cursor Column

Reports the column value of the V5 Brain's screen cursor location.

```don
brain.screen.column()
```

## How To Use

Screen column reports a range from **1 to 80**.

The V5 Brain allows you to change the size of the font printed on the screen. Changing the font will affect the number of columns available on the V5 Brain's screen.

**V5 Brain Font Size - Number of Columns:**

* `FontType.MONO12` - 80 Columns
* `FontType.MONO15` - 68 Columns
* `FontType.MONO20` / `FontType.PROP20` - 48 Columns (Default)
* `FontType.MONO30` / `FontType.PROP30` - 32 Columns
* `FontType.MONO40` / `FontType.PROP40` - 24 Columns
* `FontType.MONO60` / `FontType.MONO60` - 16 Columns
	
<advanced>
</advanced>
