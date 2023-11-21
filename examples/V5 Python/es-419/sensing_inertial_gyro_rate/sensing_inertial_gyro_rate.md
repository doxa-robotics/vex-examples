category: sensing  
signature: inertial.gyro_rate(AxisType.XAXIS, RPM)
description:  Gets the rate of rotation from one of the axes (x, y, or z) on the Inertial Sensor.

# Tasa de Giroscopio Inercial

Obtiene la velocidad de rotación de uno de los ejes (x, y o z) en el Sensor Inercial.

```don
inertial.gyro_rate(AxisType.XAXIS, RPM)
```

## Cómo Utilizar

La velocidad de giro indica un rango de **-1000.0 a 1000.0** en dps (grados por segundo).

Elija qué eje utilizar.

* El X-Axis (Eje X) informa de la velocidad de rotación cuando el sensor inercial gira en el eje X (basado en la orición del sensor)
* El X-Axis (Eje Y) informa de la velocidad de rotación cuando el sensor inercial gira en el eje Y (basado en la orición del sensor)
* El X-Axis (Eje Z) informa de la velocidad de rotación cuando el sensor inercial gira en el eje Z (basado en la orición del sensor)


<advanced>
</advanced>
