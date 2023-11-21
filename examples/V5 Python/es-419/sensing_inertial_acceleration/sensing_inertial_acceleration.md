category: sensing  
signature: inertial.acceleration(AxisType.XAXIS)
description:  Reports the acceleration value from one of the axes (x, y, or z) on the Intertial Sensor.

# Aceleración Inercial

Reporta del valor de aceleración de uno de los ejes (x, y o z) en el Sensor Intertial.

```don
inertial.acceleration(AxisType.XAXIS)
```

## Cómo Utilizar

Aceleración informa de un rango de **-4.0 a 4.0 Gs**.

Choose which axis to use:

* El X-axis (Eje-X) informa de la aceleración cuando el sensor interial se mueve **lado a lado**
* El Y-axis (Eje-Y) informa de la aceleración cuando el sensor interial se mueve **de arriba a abajo**
* El Z-axis (Eje-Z) informa de la aceleración cuando el sensor interial se mueve **hacia adelante hasta atrás**


<advanced>
</advanced>
