category: looks  
signature: CONTROLLER.Screen.newLine();  
device_class: controller  
description: Sets the print output cursor on the V5 Controller's screen to the next available row.  

# Ohjaimen kursori uudelle riville

Asetaa tulostusta varten kursorin uudelle riville ohjaimen näytöllä.

```cpp
Controller.Screen.newLine();
```

## Miten käytetään

Oletuksena ohjelman alussa kursori on rivillä 1 sarakkeessa 1. `Controller.Screen.newLine();` komennolla kursori siirtyy seuraavalle riville ohjaimen näytöllä rivin ensimmäiselle sarakkeelle.

---

V5 ohjainen näytön tulostusfonttia ei voi muuttaa.

**V5 Ohjaimen fonttikoko - Rivien määrä:**

* Standardi Fontti - 3 riviä (oletus)

![controller_screen_info](v5_controller_rows_columns.jpg)

<advanced>
</advanced>