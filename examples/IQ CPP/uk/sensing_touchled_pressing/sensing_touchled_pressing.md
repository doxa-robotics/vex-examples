category: sensing  
signature: TouchLED.pressing()  
device_class: TouchLED
description: Reports if the VEX IQ Touch LED is pressed. 

# TouchLED Pressing

Повідомляє, якщо LED датчик дотику натиснуто.

```cpp
TouchLED.pressing()
```

## Як це працює

Передає значення **true**, якщо обраний LED датчик дотику натиснуто. Передає значення **false**, якщо обраний LED датчик дотику не натиснуто.

Перша частина команди - назва пристрою.

```cpp
TouchLED2.pressing()
TouchLED4.pressing()
```

## Приклад

Приклад нижче надає LED датчику дотику червоний колір **red**. Коли LED датчику дотику натиснути, його колір зміниться на зелений **green**.

```cpp
TouchLED.setColor(red);

while (!TouchLED.pressing()) {
  wait(20, msec);
}

TouchLED.setColor(green);
```

<advanced>
</advanced>