category: sensing  
signature: inertial.calibrate()
description: Gets the rate of rotation from one of the axes (x, y, or z) on the Inertial Sensor.

# Calibrar Sensor Inercial
 
Calibración del Sensor Inercial se utiliza para reducir la cantidad de deriva generada por el Sensor Inercial.

```don
inertial.calibrate()
```

La deriva se produce cuando el Sensor Inercial detecta incorrectamente el movimiento aunque el sensor no se esté moviendo físicamente.

## Cómo Utilizar

El Sensor Inercial debe permanecer inmóvil durante el proceso de calibración. El proceso de calibración tardará aproximadamente 2 segundos en completarse.


<advanced>
</advanced>
