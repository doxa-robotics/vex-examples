category: looks  
signature: brain.screen.draw_rectangle(1, 1, 10, 10)  
description: Draws a rectangle on the V5 Brain's screen.  

# Dibujar Rectángulo

Dibuja un rectángulo en la pantalla del V5 Brain.

```don
brain.screen.draw_rectangle(X, Y, WIDTH, HEIGHT)
```

## Cómo Utilizar

El comando `brain.screen.draw_rectangle()` requiere 4 valores:

* Value 1: Top Left Corner X coordinate (Coordenada X de la esquina superior izquierda)
* Value 2: Top Left Corner Y coordinate (Coordenada Y de la esquina superior izquierda)
* Value 3: Width of the rectangle (Ancho del rectángulo)
* Value 4: Height of the rectangle (Altura del rectángulo)

El color de la línea de borde del rectángulo viene determinado por el comando `brain.screen.set_pen_color()`. El color de línea predeterminado es blanco.

El color de relleno interior del rectángulo se determina mediante el comando `brain.screen.set_fill_color()`. El color de relleno predeterminado es negro.

![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>
