category: motion  
signature: motor.spin_to_position(90, DEGREES)
description: Spins a V5 Smart Motor to a certain position.

# Girar a la Posición

Establece la posición del codificador del V5 Smart Motor en la cantidad dada.

```don 
motor.spin_to_position(AMOUNT, UNIT)
```

## Cómo Utilizar

Este mando le indicará al motor que se desplace a una posición específica. Basado en la posición actual del Motor, `spin_to_position` determinará la dirección de rotación.

Elija la unidad de medida para que sea **DEGREES** (Grados) o **TURNS** (Vueltas).

Elija si este comando debe ser esperado o no por otros comandos, cambiando el tercer parámetro opcional a **wait=True** (espera) o **wait=False** (no espera).

```don
motor.spin_to_position(90, DEGREES, wait=False)
```

Establecer **wait=True** (espera) significa que los comandos de procedimiento no se ejecutarán hasta que se complete el giro del motor. En cambio, **wait=False** (no espera) no esperará a que se complete.  

Por defecto, este comando tendrá la espera que se establecerá en **True**.

<advanced>
</advanced>
