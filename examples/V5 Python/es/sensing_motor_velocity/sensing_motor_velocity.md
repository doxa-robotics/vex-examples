category: sensing  
signature: motor.velocity(PERCENT)
description: Reports the current velocity of a V5 Smart Motor.

# Velocidad del Motor

Reporta de la velocidad actual de un V5 Smart Motor.

```don
motor.velocity(UNIT)
```

## Cómo Utilizar

Velocidad del Motor reporta un rango de **-100% a 100%** o **-600rpm a 600rpm**.

Los valores aceptables para el parámetro 'UNIT' (Unidad) son: **DEGREES** (Grados) o **RPM**.

Velocidad del Motor reportará de un rango de "rotaciones por minuto" basado en el cartucho de engranajes instalado en los V5 Smart Motor.

* Red Cartridge (Cartucho Rojo): -100rpm a 100rpm
* Green Cartridge (Cartucho Verde): -200rpm a 200rpm
* Blue Cartridge (Cartucho Azul): -600rpm a 600rpm


<advanced>
</advanced>
