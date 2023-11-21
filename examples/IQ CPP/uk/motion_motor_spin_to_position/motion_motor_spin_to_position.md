category: motion  
signature: Motor.spinToPosition(90, degrees);  
device_class: motor  
description: Spins the motor to a position.  

# Spin Motor To Position

Повертає мотор VEX IQ у певну позицію.

```cpp
Motor.spinToPosition(rotation, units);
```

## Як це працює

Команда `Motor.spinToPosition` повідомляє мотору, в яку позицію прокрутитися. Зважаючи на поточну позицію мотора, `Motor.spinToPosition` сама обере напрямок обертання.

Команда `Motor.spinToPosition` приймає числові значення для параметра `rotation`.

Встановіть одиниці вимірювання `units` для обертання в  **degrees** або **turns**. 

Команда `Motor.spinToPosition` блокує інші команди, поки мотор не прокрутиться на задану величину.

## Необов'язкові параметри

Ви можете встановити значення останнього параметра `false`, щоб команда `Motor.spinToPosition` не блокувала програму під час виконання руху.

```cpp
Motor.spinToPosition(360, degrees, false);
```

<advanced>
</advanced>