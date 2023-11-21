category: looks  
signature: brain.screen.draw_circle(1, 1, 10)  
description: Draws a circle on the V5 Brain's screen.  

# Dibujar Círculo

Dibuja un círculo en la pantalla del V5 Brain.

```don
brain.screen.draw_circle(X, Y, RADIUS)
```

## Cómo Utilizar

El comando `brain.screen.draw_circle()` requiere 3 valores:

* Value 1: Center Point X
* Value 2: Center Point Y
* Value 3: Radius of Circle (in pixels) (Radio de círculo (en pixels))

El color de la línea exterior del círculo se determina por el comando `brain.screen.set_pen_color()`. El color de línea predeterminado es blanco.

El color color de relleno interior del círculo se determina por el comando `brain.screen.set_fill_color()`. El color de relleno predeterminado es negro.

![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>
