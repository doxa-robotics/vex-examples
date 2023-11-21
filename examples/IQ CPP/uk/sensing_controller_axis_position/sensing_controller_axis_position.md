category: sensing  
signature: Controller.Axis.position()  
device_class: controller  
description: Reports the position of a joystick on the IQ Controller along an axis.  

# Controller Axis Position

Передає позицію джойстика на контролері VEX IQ уздовж заданої вісі.

```cpp
Controller.Axis.position()
```

## Як це працює

`Controller.Axis.position` передає значення в діапазоні **від -100 до 100**.

`Controller.Axis.position` передасть **0**, коли вісь джойстика посередині.

Виберіть, яку вісь контролера передавати:

* `AxisA` - лівий джойстик (вгору і вниз)
* `AxisB` - лівий джойстик (вліво і вправо)
* `AxisC` - правий джойстик (вліво і вправо)
* `AxisD` - правий джойстик (вгору і вниз)

## Приклад

Приклад нижче надрукує позицію вісі А контролера на екрані VEX IQ Brain.

```cpp
while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("AxisA Position: %.0f", Controller.AxisA.position());

  // Коротка затримка запобігає ривкам або перериванням
  wait(20, msec);
}

```

<advanced>
</advanced>