category: looks  
signature: CONTROLLER.Screen.setCursor(1, 1);  
device_class: controller  
description: Sets the cursor location for **Controller.Screen.print();** command on the V5 Controller's screen.

# Aseta kursoripaikka


Asettaa kursorin paikan ohjaimen näytöllä komentoa **Controller.Screen.print();** varten.

```cpp
Controller.Screen.setCursor(1, 2);
```


## Miten käytetään

Komento `controller.screen.setCursor()` vaatii 2 arvoa:

* Value 1: Näytön rivi 
* Value 2: Näytön sarake

Asettamalla kursoriksi sopiva rivi ja sarake saat tulostettua komennolla `controller.screen.print()` haluttuun kohtaan näyttöä.

`Controller.Screen.setCursor();` hyväksyy rivin **row** välillä **1 - 3**.

`Controller.Screen.setCursor();` hyväksyy sarakkeen **column** välillä **1 - 20**.

---

V5 Ohjainnäytölle ei voi muuttaa fontin kokoa.

**V5 Ohjain Fontin koko - Rivien määrä:**

* Standard Fontti - 3 riviä (Oletus)

**V5 Ohjain Fontin koko - Sarakkeiden määrä**

* Standard Fontti - 20 Saraketta (Oletus)
* Value 1: Screen row position 
* Value 2: Screen column position


![controller_screen_info](v5_controller_rows_columns.jpg)

<advanced>
</advanced>