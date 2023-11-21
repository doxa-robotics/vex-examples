category: looks  
signature: brain.screen.new_line()  
description: Sets the print output cursor on the V5 Brain's screen to the next available row.  

# Siguiente fila

Establece el cursor de salida de impresión en la pantalla del V5 Brain a la siguiente fila disponible.

```don
brain.screen.new_line()
```

## Cómo Utilizar

Por defecto, todos los proyectos comienzan con el cursor de la pantalla en la fila 1 columna 1. El comando `brain.screen.new_line()` moverá el cursor hacia abajo una sola fila en la pantalla. `brain.screen.new_line()` también establecerá la columna del cursor en la posición 1.

---

El V5 Brain permita cambiar el tamaño de la fuente impresa en la pantalla. Changing the font will affect the number of rows available on the V5 Brain's screen.

**Tamaño de fuente del V5 Brain - Número de Filas:**

* `FontType.MONO12` - 20 Filas
* `FontType.MONO15` - 16 Filas
* `FontType.MONO20` / `FontType.PROP20` - 12 Filas (Por Defecto)
* `FontType.MONO30` / `FontType.PROP30` - 8 Filas
* `FontType.MONO40` / `FontType.PROP40` - 6 Filas
* `FontType.MONO60` / `FontType.PROP60` - 4 Filas

![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>
