category: looks  
signature: Brain.Screen.clearScreen();  
description: Clears the entire V5 Brain screen.  

# Clear Screen

Очищує весь екран VEX IQ Brain.

```cpp
Brain.Screen.clearScreen();
```

## Як це працює

`Brain.Screen.clearScreen` не скидає позицію курсора на екрані Brain 

Використовуйте команду `Brain.Screen.setCursor`, щоб встановити бажану позицію курсора на Brain.

## Приклад

Цей приклад надрукує "Hello", почекає одну секунду, а потім очистить весь екран перед друком "Goodbye".

```cpp
Brain.Screen.print("Hello");
wait(1.0, seconds);
Brain.Screen.clearScreen();
Brain.Screen.print("Goodbye");
```

<advanced>
</advanced>