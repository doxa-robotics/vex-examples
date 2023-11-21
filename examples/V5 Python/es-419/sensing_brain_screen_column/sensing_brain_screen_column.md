category: sensing  
signature: brain.screen.column()  
description: Reports the column number of the V5 Brain screen cursor location.

# Columna del Cursor

Informa del valor de columna de la ubicación del cursor de pantalla del V5 Brain.

```don
brain.screen.column()
```

## Cómo Utilizar

La columna de pantalla informa de un rango de **1 a 80**.

El V5 Brain permita cambiar el tamaño de la fuente impresa en la pantalla. Cambiar la fuente afectará al número de columnas disponibles en la pantalla del V5 Brain.

**Tamaño de fuente del V5 Brain- Número de columnas:**

* `FontType.MONO12` - 80 Columnas
* `FontType.MONO15` - 68 Columnas
* `FontType.MONO20` / `FontType.PROP20` - 48 Columnas (por defecto)
* `FontType.MONO30` / `FontType.PROP30` - 32 Columnas
* `FontType.MONO40` / `FontType.PROP40` - 24 Columnas
* `FontType.MONO60` / `FontType.MONO60` - 16 Columnas
	
<advanced>
</advanced>
