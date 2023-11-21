category: looks  
signature: CONTROLLER.Screen.clearLine();  
device_class: controller  
description: Clears a single row on the V5 Controller's screen.  

# Tyhjää ohjaimen näytön rivi

Tyhjää ohjaimen näytön.
```cpp
Controller.Screen.clearLine(1);
```

## Miten käytetään

`Controller.Screen.clearLine();` ei muuta kursoripaikkaa näytöllä. 

Halutessasi käytä `Controller.Screen.clearLine();` komentoa asettamaan kursorin haluttuun rivipaikkaan välillä **1 - 3**.

```cpp
Controller.Screen.clearLine();
```

Tyhjää tietyn rivin .

```cpp
Controller.Screen.clearLine(1);
```

V5 Ohjaimen näytöllä ei voi muuttaa fonttikokoa.

**V5 Ohjain fonttikoko - Rivimäärä:**

* Standardi Fontti - 3 riviä (Oletus)

![controller_screen_info](v5_controller_rows_columns.jpg)

<advanced>
</advanced>