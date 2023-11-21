category: looks  
signature: controller.screen.new_line()  
description: Sets the print output cursor on the V5 Controller's screen to the next available row.  

# Siguiente Fila

Establece el cursor de salida de impresión en la pantalla del controlador V5 en la siguiente fila disponible.

```don
controller.screen.new_line()
```

## Cómo Utilizar

De forma predeterminada, todos los proyectos comienzan con el cursor de la pantalla en la fila 1, columna 1. El comando `controller.screen.new_line()` moverá el cursor hacia abajo por una sola fila en la pantalla. `controller.screen.new_line()` también establecerá la columna del cursor en la posición 1.

---

El V5 Controller no permita cambiar el tamaño de la fuente impresa en la pantalla.

**Tamaño de fuente del V5 Brain - Número de filas:**

* Standard Font (Fuente Estándar) - 3 Filas (por defecto) 

**Tamaño de fuente del V5 Controller - Número de columnas:**

* Standard Font (Fuente Estándar) - 20 Columnas (por defecto)

![controller_screen_info](v5_controller_rows_columns.jpg)

<advanced>
</advanced>
