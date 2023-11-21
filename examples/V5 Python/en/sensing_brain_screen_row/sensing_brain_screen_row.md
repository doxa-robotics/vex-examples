category: sensing  
signature: brain.screen.row()  
description: Reports the row number of the V5 Brain screen cursor location.

# Cursor Row
 
Reports the row value of the V5 Brain's screen cursor location.

```don
brain.screen.row()
```

## How To Use

Screen row reports a range from **1 to 20**.

The V5 Brain allows you to change the size of the font printed on the screen. Changing the font will affect the number of rows available on the V5 Brain's screen.

**V5 Brain Font Size - Number of Rows:**

* `FontType.MONO12` - 20 Rows
* `FontType.MONO15` - 16 Rows
* `FontType.MONO20` / `FontType.PROP20` - 12 Rows (Default)
* `FontType.MONO30` / `FontType.PROP30` - 8 Rows
* `FontType.MONO40` / `FontType.PROP40` - 6 Rows
* `FontType.MONO60` / `FontType.PROP60` - 4 Rows
	
<advanced>
</advanced>
