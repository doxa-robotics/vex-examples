category: looks  
signature: controller.screen.new_line()  
description: Sets the print output cursor on the V5 Controller's screen to the next available row.  

# Seuraava rivi

Siirtää V5 ohjaimen näytöllä kursorin seuraavalle riville.

```don
controller.screen.next_row()
```

## Miten käytetään

Oletuksena kursori on aina ohjelman alussa sivillä1 sarakkeessa 1. Komento `controller.screen.next_row()` siirtää kutsoria yhden rivi alas näytöllä sarakkeeseen 1.

---

V5 Ohjain ei salli muuttaa tulostuksen kirjasinta.

**V5 Ohjain Fontti Koko - Rivien määrä:**

* Standard Fontti - 3 riviä (Oletus)

**V5 Ohjain Fontti Koko - Sarakkeiden määrä:**

* Standard Fontti - 20 saraketta (Oletus)

![controller_screen_info](v5_controller_rows_columns.jpg)

<advanced>
</advanced>
