category: sensing  
signature: gyro.set_heading(0, DEGREES)
description: Sets the Gyroscopic (Gyro) sensor's current heading position to a set value.

# Establecer Dirección de Giroscopio

Establecer la dirección actual del Sensor Giroscópico (Gyro) en un valor establecido.
 
```don
gyro.set_heading(HEADING, DEGREES)
```

## Cómo Utilizar

El comando establecer dirección de giroscopio se puede utilizar para establecer la posición del giroscopio en cualquier dirección en el sentido de las agujas del reloj.

Este comando se utiliza normalmente para restablecer la dirección del sensor Gyro cuando el valor se establece en 0.

El parámetro 'HEADING' (dirección) acepta un rango de **0.0 a 359.99 grados**.

El comando establecer dirección puede aceptar decimales, enteros o valores numéricos.

<advanced>
</advanced>
