category: looks  
signature: Brain.Screen.print("Hello");  
description: Prints values or text on the IQ Brain's screen.  

# Print

Друкує значення або текст на екрані VEX IQ Brain.

```cpp
Brain.Screen.print();
```

## Як це працює

Команда `Brain.Screen.print` надрукує дані з позиції курсора на екрані Brain.

Всі нові проєкти починають із курсором в рядку 1 стовпці 1.

Друкує слова або числа.:
```cpp
Brain.Screen.print("String: 123 + Words");
```

Друкує цілі або десяткові значення:
```cpp
// Коли друкується ціле число, потрібен специфікатор формата
// "%d" у першому параметрі

Brain.Screen.print("Integer: %d", 5 + 10);

// Коли друкується десяткове число, потрібен специфікатор формата
// "%f" у першому параметрі

Brain.Screen.print("Decimal: %f", 5.0 + 10.0);
```

Друкує значення команд показників датчиків:
```cpp
// Якщо вихідне значення ціле або десяткове число, використайте
// "%f" або "%d" відповідно як специфікатор формата

Brain.Screen.print("%d", Brain.Timer.time());

// Якщо вихідне значення булеве (логічне),
// використайте "%s" як специфікатор формата

Brain.Screen.print("%s", Motor.isDone() ? "TRUE" : "FALSE");
```

<advanced>
</advanced>