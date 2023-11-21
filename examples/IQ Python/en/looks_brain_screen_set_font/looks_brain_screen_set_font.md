category: looks  
signature: brain.screen.set_font(FONT)  
description: Sets the style and size of font used on the IQ (2nd generation) Brain's screen when printing numbers or text  

# Brain Screen Set Font

Sets the style and size of font used on the IQ (2nd generation) Brain's screen when printing numbers or text.

```python
brain.screen.set_font(FONT)
```

## How To Use

There are two different types of fonts available on the IQ (2nd generation) Brain's screen:

* Monospaced (Mono) - each character takes up the same width.
* Proportional (Prop) - each character takes up different size widths based on the character.

Choose which font type and size to use. You can replace the **FONT** parameter with one of the following font options:

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

The new font size will be used for any future text written to the IQ (2nd generation) Brain's screen.

<advanced>
</advanced>