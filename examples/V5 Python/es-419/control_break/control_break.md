category: control  
signature: break  
description: Exits a repeating loop immediately.

# Romper

Sale de un bucle de repetición inmediatamente.

```don
break
```

## Cómo Utilizar

Cuando se añade dentro de un bucle, la orden de 'break' saldrá del bucle del que se está ejecutando actualmente. 

## Ejemplo

Este ejemplo accionará el robot y comprobará si se ha pulsado su 'bumper'.

Si el parachoques se **presiona**, la orden de 'break' saldrá del bucle while. El robot dejará de conducir hacia adelante.

```don
while True:
    drivetrain.drive(FORWARD)
    if bumper.pressing():
        break
```
<advanced>
</advanced>
