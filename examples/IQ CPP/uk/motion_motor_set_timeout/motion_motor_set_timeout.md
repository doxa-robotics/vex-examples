category: motion  
signature: Motor.setTimeout(1, seconds);  
device_class: motor  
description: Sets the Motor's timeout to stop if a blocking command never reaches its target.  

# Motor Set Timeout

Встановлює часові обмеження на всі команди руху мотора, щоб зупинити його, якщо команда мотора блокує роботу і не може досягти своєї цілі.  

```cpp
Motor.setTimeout(time, seconds);
```

## Як це працює

Команда `Motor.setTimeout` потрібна, щоб команди руху, які не змогли досягти своєї позиції, не заважали працювати наступним командам.

Приклад мотору, який не досягнув своєї позиції - клешня або рука, яка зіштовхнулась із механічними обмеженнями і не може закінчити свій рух.

Встановіть часові обмеження, задавши кількість часу в секундах **seconds**.

## Приклад

Цей приклад зупинить команду `Motor.spinToPosition` через 2 секунди, якщо ClawMotor не встигне досягти позиції 270 градусів. 

Щойно часові обмеження або обертання будуть подолані, ClawMotor обертатиметься до позиції 90 градусів.

```cpp
ClawMotor.setTimeout(2, seconds);
ClawMotor.spinToPosition(270, degrees);
ArmMotor.spinToPosition(90, degrees);
```

<advanced>
</advanced>