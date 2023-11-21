category: looks  
signature: brain.screen.set_font(FontType.MONO20)  
description: Sets the style and size of font used on the V5 Brain's screen when printing numbers or text.  

# Aseta fontti/kirjasinlaji

Asettaa kirjasimen koon ja tyylin V5 Aivojen näytölle tulostettaessa.

```don
brain.screen.set_font(FONT_TYPE)
```

## Miten käytetään

Käytössä on kaksi eri kirjasinlajia:

* Monospaced (MONO) - kirjaimet ovat saman levyisiä.
* Proportional (PROP) - jokainen kirjaimella oma leveys.

Valitse kirjasinlaji ja koko , jota käytät `FONT_TYPE` parametrina:

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

Fontti säilyy käytössä kunnes vaihdat sen uuteen tulostettaessa.

<advanced>
</advanced>
