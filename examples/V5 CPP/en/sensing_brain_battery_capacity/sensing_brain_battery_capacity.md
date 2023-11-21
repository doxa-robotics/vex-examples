category: sensing  
signature: Brain.Battery.capacity()  
description: Reports the capacity of the V5 Brain's battery.

# Brain Battery Capacity

Reports the capacity of the V5 Brain's battery.

```cpp
Brain.Battery.capacity()
```

## How To Use
Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

`Brain.Battery.capacity()` returns an **integer** that represents the Battery's capacity in the default unit of `percent`, and will return a value in the range of **0% to 100%**.

```cpp
Brain.Screen.print("%d", Brain.Battery.capacity());
```

<advanced>
</advanced>