category: motion  
signature: Motor.stop();  
device_class: motor  
description: Stops a motor.  

# Stop Motor

Зупиняє мотор.

```cpp
Motor.stop();
```

## Як це працює

Перша частина команди - назва пристрою.
```cpp
ClawMotor.stop();
ArmMotor.stop();
``` 

## Приклад

Цей приклад обертатиме мотор 3 секунди до зупинки.

```cpp
ClawMotor.spin(forward);
wait(3, seconds);
ClawMotor.stop();
```

<advanced>
</advanced>