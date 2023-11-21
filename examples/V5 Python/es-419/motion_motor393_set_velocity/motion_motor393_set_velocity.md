category: motion  Use
signature: motor393.set_velocity(10, PERCENT)  
description: Sets the speed of a Motor 393.

# Establecer la Velocidad del Controlador del Motor

Establece la velocidad de un Motor 393 conectado a un Controlador de Motor 29.

```don 
motor393.set_velocity(VELOCITY, PERCENT)
```

## Cómo Utilizar

El parámetro 'VELOCITY' (Velocidad) acepta un rango de -100% a 100%.

Si se establece la velocidad de un Motor 393 en un valor negativo hará que el Motor 393 gire en reversa.

La secuencia siguiente hará que el Motor 393 gire en sentido inverso, aunque se pase el parámetro 'FORWARD' (Adelante).

```don
motor393.set_velocity(-100, PERCENT)
motor393.spin(FORWARD)
```

Ajustar la velocidad de un Motor 393 a 0 evitará que el Motor gire.


<advanced>
</advanced>
