category: motion  
signature: Motor.spinFor(forward, 90, degrees);  
device_class: Motor  
description: Spins the motor for a number of degrees or turns.  

# Spin Motor For

Повертає мотор VEX IQ на певну величину.

```cpp
Motor.spinFor(direction, rotation, units);
```

## Як це працює

`Motor.spinFor` обертає мотор у заданий бік і на задану відстань.

Можливі параметри:

- `direction` приймає значення напрямку **forward** або **reverse**
- `rotation` приймає числові значення величини повороту
- `units` приймає значення одиниць **degrees** або **turns**

Команда `Motor.spinFor` блокує інші команди, поки мотор не прокрутиться на задану величину.

## Необов'язкові параметри

Ви можете встановити значення останнього параметра `false`, щоб команда `Motor.spinFor` не блокувала програму під час виконання руху.

```cpp
Motor.spinFor(reverse, 360, degrees, false);
```

<advanced>
</advanced>
