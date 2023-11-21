category: sensing  
signature: Gyro.setHeading(heading, degrees);  
device_class: gyro  
description: Sets the Gyroscopic (Gyro) sensor's current heading to the value provided. 

# Gyro Set Heading

Встановлює поточну позицію курсу гіроскопічного датчика у задане значення.

```cpp
Gyro.setHeading(heading, degrees);
```

## Як це працює

`Gyro.setHeading` використовують, щоб перезаписати поточну позицію курсу гіродатчика на значення в діапазоні від **0** до **359.99**. 

Цю команду зазвичай використовують, щоб скинути значення курсу гіродатчика в 0.

`Gyro.setHeading` може приймати десяткові або цілі значення.

## Приклад

Частина коду нижче встановлює значення курсу гіродатчика в 0 градусів.

```cpp
Gyro.setHeading(0, degrees);
```

<advanced>
</advanced>