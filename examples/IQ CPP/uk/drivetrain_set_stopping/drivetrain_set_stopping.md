category: drive  
signature: Drivetrain.setStopping(brake);  
device_class: drivetrain  
description: Sets the brake mode of the Drivetrain.  

# Set Stopping

Встановлює режим гальмування трансмісії

```cpp
Drivetrain.setStopping(brakeType);
```

## Як це працює

Ось можливі вхідні значення для параметра `brakeType`, які ви можете задати: 

* **brake** змушує трансмісію миттєво зупинитися і не реагувати на зовнішні сили.
* **coast** дає змогу трансмісії поступово зменшити оберти до зупинки.
* **hold** змушує трансмісію миттєво зупинитися і повертатиме її до позиції зупинки, якщо діють зовнішні сили.

## Приклад

Цей приклад змушує трансмісію їхати вперед 3 секунди, а потім утримувати позицію після зупинки.

```cpp
Drivetrain.setStopping(hold);
Drivetrain.drive(forward);
wait(3, seconds);
Drivetrain.stop();
```

<advanced>
</advanced>