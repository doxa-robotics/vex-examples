category: sensing  
signature: brain.screen.row()  
description: Reports the row number of the V5 Brain screen cursor location.

# Fila del Cursor
 
Reporta del valor de fila de la ubicación del cursor de pantalla del V5 Brain.

```don
brain.screen.row()
```

## Cómo Utilizar

La fila de pantalla informa de un rango de **1 a 20**.

El V5 Brain permita cambiar el tamaño de la fuente impresa en la pantalla. Cambiar la fuente afectará al número de filas disponibles en la pantalla del V5 Brain.

**Tamaño de fuente del V5 Brain - Número de filas:**

* `FontType.MONO12` - 20 Filas
* `FontType.MONO15` - 16 Filas
* `FontType.MONO20` / `FontType.PROP20` - 12 Filas (por defecto)
* `FontType.MONO30` / `FontType.PROP30` - 8 Filas
* `FontType.MONO40` / `FontType.PROP40` - 6 Filas
* `FontType.MONO60` / `FontType.PROP60` - 4 Filas
	
<advanced>
</advanced>
