category: looks  
signature: brain.screen.set_cursor(1, 1)
description: Sets the cursor location for brain.screen.print() command on the V5 Brain's screen.

# Establecer Cursor


Establece la ubicación del cursor en la pantalla del V5 Brain.

```don
brain.screen.set_cursor(ROW, COLUMN)
```

## Cómo Utilizar

El comando `brain.screen.set_cursor()` requiere 2 valores:

* Value 1: Screen row position (Posición de la fila de la pantalla)
* Value 2: Screen column position (Posición de la columna de la pantalla)

Establezca la posición de fila y columna del cursor para que se muestre un comando `brain.screen.print()` en una ubicación específica de la pantalla.

Acepta un rango para **fila** de **1 a 20**.

Acepta un rango para **columna** de **1 a 80**.

---

El cerebro V5 le permite cambiar el tamaño de la fuente impresa en la pantalla. Cambiar la fuente afectará al número de filas y columnas disponibles en la pantalla del V5 Brain.

**V5 Brain Tamaño De Fuente - Número de Filas:**

* `FontType.MONO12` - 20 Rows (Filas)
* `FontType.MONO15` - 16 Rows (Filas)
* `FontType.MONO20` / `FontType.PROP20` - 12 Rows (Default) (Filas - Por Defecto)
* `FontType.MONO30` / `FontType.PROP30` - 8 Rows (Filas)
* `FontType.MONO40` / `FontType.PROP40` - 6 Rows (Filas)
* `FontType.MONO60` / `FontType.PROP60` - 4 Rows (Filas)

**V5 Brain Tamaño De Fuente - Número de Columnas:**

* `FontType.MONO12` - 80 Columns (Columnas)
* `FontType.MONO15` - 68 Columns (Columnas)
* `FontType.MONO20` / `FontType.PROP20` - 48 Columns (Default) (Columnas - Por Defecto)
* `FontType.MONO30` / `FontType.PROP30` - 32 Columns (Columnas)
* `FontType.MONO40` / `FontType.PROP40` - 24 Columns (Columnas)
* `FontType.MONO60` / `FontType.MONO60` - 16 Columns (Columnas)

![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>
