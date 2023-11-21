category: looks  
signature: brain.screen.clear_line()  
description: Clears a single row on the V5 Brain screen.  

# Borrar Fila

Borra una sola fila en la pantalla del V5 Brain o Controller.

```don 
brain.screen.clear_line()
```

## Cómo Utilizar

Borra la fila actual en la pantalla V5 Brain.

```don
brain.screen.clear_line()
```

Borra una fila especificada en la pantalla del V5 Brain.

```don
brain.screen.clear_line(ROW)
```

## Cómo Utilizar

El comando `brain.screen.clear_line()` puede aceptar valores enteros entre **1 - 20**, para establecer qué fila se va a borrar. También se puede llamar al comando sin ningún argumento para borrar la fila actual.

---

![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>
