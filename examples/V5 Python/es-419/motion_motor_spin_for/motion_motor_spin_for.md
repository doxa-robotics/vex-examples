category: motion  
signature: motor.spin_for(FORWARD, 90, DEGREES)  
description: Spins a V5 Smart Motor for a given distance.

# Girar Por
 
Este comando hace girar un V5 Smart Motor durante una cantidad determinada de grados o giros.

```don
motor.spin_for(DIRECTION, AMOUNT, UNIT)
```

## Cómo Utilizar

Elija a qué 'DIRECTION' (Dirección) girará el motor: **FORWARD** (Adelante) o **REVERSE** (Hacia Atras).

Elija la 'UNIT' (UNIDAD) de medida para que sea **DEGREES** (Grados) o **TURNS** (Vueltas).

Elija si este comando debe ser esperado o no, siguiendo los comandos estableciendo un cuarto parámetro opcional en **wait=True** (espera) o **wait=False** (no espera). 

```don
motor.spin_for(FORWARD, 90, DEGREES, wait=False)
```

Este comando es un comando de bloqueo a menos que **wait-False** (no espera) se pase como el cuarto parámetro.

<advanced>
</advanced>
