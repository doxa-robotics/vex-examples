category: looks  
signature: controller.screen.clear_line()  
description: Clears a single row on the V5 Controller's screen.  

# Borrar Fila

Borra la fila actual en la pantalla del V5 Controller.

```don
controller.screen.clear_line()
```

Borra una fila especificada en la pantalla del V5 Contoller.

```don
controller.screen.clear_line(ROW)
```

## Cómo Utilizar

El comando `controller.screen.clear_line()` puede aceptar valores enteros entre **1 - 3**, para establecer qué fila se va a borrar. También puede llamar al comando sin argumentos para borrar la fila actual.

---

El V5 Controller no permite cambiar el tamaño de la fuente impresa en la pantalla.

**V5 Controller Font Size - Number of Rows:**

* Standard Font - 3 Rows (Default)

![controller_screen_info](v5_controller_rows_columns.jpg)

<advanced>
</advanced>
