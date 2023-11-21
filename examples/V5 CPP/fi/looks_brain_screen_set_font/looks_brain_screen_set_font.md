category: looks  
signature: Brain.Screen.setFont(monoM);  
description: Sets the style and size of font used on the V5 Brain's screen when printing numbers or text.  

# Brain Screen Set Font

Sets the style and size of font used on the V5 Brain's screen when printing numbers or text.

```cpp
Brain.Screen.setFont(monoM);
```

## How To Use

There are two different types of fonts available on the V5 Brain's screen:

* Monospaced (Mono) - each character takes up the same width.
* Proportional (Prop) - each character takes up different size widths based on the character.

Choose which font type and size to use. You can select from the following font options.

* `mono12`
* `mono15`
* `mono20`
* `mono30`
* `mono40`
* `mono60`
* `prop20`
* `prop30`
* `prop40`
* `prop60`

The new font size will be used for any future text written to the V5 Brain's screen.

<advanced>
</advanced>