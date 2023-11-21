category: sensing  
signature: drivetrain.velocity(PERCENT)
description: Reports the current velocity of the Drivetrain.

# Velocidad de Conducciรณn
 
Reporta la velocidad actual del Chasis.

```don
drivetrain.velocity(UNIT)
```

## Cómo Utilizar

Velocidad de Conducciรณn reporta un rango de -100% a 100% o -600rpm a 600rpm.

El parámetro 'UNIT'(Unidad) se puede reemplazar con **PERCENT** (Por Ciento) o **RPM**.

Velocidad de Conducciรณn reportará un rango de "rotaciones por minuto" basado en el cartucho de engranajes instalado en los V5 Smart Motors utilizados en el Chasis.

* Red Cartridge (Cartucho Rojo): -100rpm to 100rpm
* Green Cartridge (Cartucho Verde): -200rpm to 200rpm
* Blue Cartridge (Cartucho Azul): -600rpm to 600rpm

<advanced>
</advanced>
