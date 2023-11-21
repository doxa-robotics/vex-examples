category: looks  
signature: brain.screen.set_font(FontType.MONO20)  
description: Sets the style and size of font used on the V5 Brain's screen when printing numbers or text.  

# Establecer Fuente

Establece el estilo y el tamaño de la fuente utilizada en la pantalla del V5 Brain al imprimir valores.

```don
brain.screen.set_font(FONT_TYPE)
```

## Cómo Utilizar

Hay dos tipos de fuentes disponibles en la pantalla del V5 Brain:

* Monospaced (MONO) - cada carácter ocupa el mismo ancho.
* Proportional (PROP) - cada carácter ocupa diferentes anchos de tamaño en función del carácter.

Elija el tipo de fuente y el tamaño que desea utilizar reemplazando el parámetro `FONT_TYPE` . Puede seleccionar entre las siguientes opciones de fuente.

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

El nuevo tamaño de fuente se utilizará para cualquier texto futuro escrito en la pantalla del V5 Brain hasta que se cambie de nuevo.

<advanced>
</advanced>
