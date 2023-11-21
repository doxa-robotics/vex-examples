category: looks  
signature: controller.screen.set_cursor(1, 1)  
description: Sets the cursor location for **controller.screen.print()** command on the V5 Controller's screen.

# Establecer cursor


Establece la ubicación del cursor para el comando **controller.screen.print()** en la pantalla del V5 Controller.

```don
controller.screen.set_cursor(ROW, COLUMN)
```

## Cómo Utilizar

El comando `controller.screen.set_cursor()` requiere 2 valores:

* Valor 1: Posición de la fila de la pantalla 
* Valor 2: Posición de la columna de pantalla


Establezca la posición de fila y columna del cursor para que se muestre un comando `controller.screen.print()` en una ubicación específica de la pantalla.

`controller.screen.set_cursor()` acepta un rango para **fila** de **1 a 3**.

`controller.screen.set_cursor()` acepta un rango para **columna** de **1 a 20**.

---

El V5 Brain no permite cambiar el tamaño de la fuente impresa en la pantalla.

**Tamaño de Fuente del V5 Controller - Número de Filas:**

* Fuente Estándar - 3 Filas (per defecto)

**Tamaño de Fuente del V5 Controller - Número de Columnas:**

* Fuente Estándar - 20 Columnas (por defecto)

![controller_screen_info](v5_controller_rows_columns.jpg)

<advanced>
</advanced>
