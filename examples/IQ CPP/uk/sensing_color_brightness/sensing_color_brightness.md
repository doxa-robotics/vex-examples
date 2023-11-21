category: sensing  
signature: Color.brightness()  
description: Reports if a button on the VEX IQ Brain is pressed.

# Color Brightness

Передає кількість світла, виміряну датчиком кольору VEX IQ.

```cpp
Color.brightness()
```

## Як це працює

`Color.brightness` передає значення в діапазоні **від 0% до 100%**.

Перша частина команди - назва пристрою.

```cpp
Color2.brightness()
Color4.brightness()
```

Більша кількість світла повертає більше числове значення, менша кількість - менше.

## Приклад

Приклад нижче друкує кількість світла, зафіксованого датчиком кольору.

```cpp
Brain.Screen.print("Brightness: %d", Color.brightness());
```

<advanced>
</advanced>
