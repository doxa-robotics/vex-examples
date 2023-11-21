category: sensing  
signature: inertial.orientation(OrientationType.ROLL , DEGREES)
description:  Gets an orientation angle of the inertial sensor. Reports the unit value specified by the parameter of the inertial sensor.

# Orientación Inercial

Obtiene un ángulo de orientación del Sensor Inercial. Informa del valor de unidad especificado por el parámetro del Sensor Inercial.

```don
inertial.orientation(OrientationType.ROLL, DEGREES)
```

## Cómo Utilizar
La orientación notificada viene determinada por el eje seleccionado (x, y, o z).

* El X-axis (Eje-x) representa el cabeceo, que informa de un valor entre -90 y +90 grados).
* El Y-axis (Eje-y) representa el rollo, que informa de un valor entre -180 y +180 grados)
* El Z-axis (Eje-z) representa la orientación, que indica un valor entre -180 y +180 grados)

<advanced>
</advanced>
