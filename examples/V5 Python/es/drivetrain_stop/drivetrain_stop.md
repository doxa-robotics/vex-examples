category: drivetrain  
signature: drivetrain.stop()  
description: Stops the Drivetrain.  

# Parar

Para el chasis.

```don
drivetrain.stop()
```

## Cómo Utilizar

El comando 'drivetrain.stop()' detiene el chasis. No toma ningún argumento entre paréntesis.

## Ejemplo

Este ejemplo detendrá el chasis después de que el V5 Robot haya conducido hacia adelante durante 3 segundos.

```don
drivetrain.drive(FORWARD)
wait(3, SECONDS)
drivetrain.stop()
```

<advanced>
</advanced>
