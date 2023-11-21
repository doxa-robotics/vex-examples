category: looks  
signature: brain.screen.set_font(FontType.MONO20)  
description: Sets the style and size of font used on the V5 Brain's screen when printing numbers or text.  

# Set Font

Sets the style and size of font used on the V5 Brain's screen when printing values.

```don
brain.screen.set_font(FONT_TYPE)
```

## How To Use

There are two different types of fonts available on the V5 Brain's screen:

* Monospaced (MONO) - each character takes up the same width.
* Proportional (PROP) - each character takes up different size widths based on the character.

Choose which font type and size to use by replacing the `FONT_TYPE` parameter. You can select from the following font options.

* `FontType.MONO12`
* `FontType.MONO15`
* `FontType.MONO20`
* `FontType.MONO30`
* `FontType.MONO40`
* `FontType.MONO60`
* `FontType.PROP20`
* `FontType.PROP30`
* `FontType.PROP40`
* `FontType.PROP60`

The new font size will be used for any future text written to the V5 Brain's screen until it is changed again.

<advanced>
</advanced>
