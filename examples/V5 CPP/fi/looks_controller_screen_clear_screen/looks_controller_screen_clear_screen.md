category: looks  
signature: CONTROLLER.Screen.clearScreen();  
device_class: controller  
description: Clears the entire V5 Controller's screen.  

# Tyhjää ohjaimen näytön rivit

Tyhjää ohjaimen näytön.

```cpp
Controller.Screen.clearScreen();
```

## Miten käytetään

`Controller.Screen.clearScreen();` ei muuta kursoripaikkaa näytöllä. 

Halutessai käytä `Controller.Screen.setCursor();` kometoa asettamaan kursorin haluttuun paikkaan.


```cpp
Controller.Screen.clearScreen();
```

<advanced>
</advanced>