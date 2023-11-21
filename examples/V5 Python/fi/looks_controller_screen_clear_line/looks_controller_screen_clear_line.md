category: looks  
signature: controller.screen.clear_line()  
description: Clears a single row on the V5 Controller's screen.  

# Tyhjää rivi

Tyhjää nykyisen rivin V5 ohjaimen näytöllä.

```don
controller.screen.clear_row()
```

Tyhjää tietyn rivin ohjaimella.

```don
controller.screen.clear_row(ROW)
```

## Miten käytetään

'controller.screen.clear_row()` komennossa hyväksytään rivinumerot **1 - 3** rivin tyhjäyksessä. Ilman numeroa tyhjätään nykyinen rivi.

---

V5 Ohjaimen näytön fonttia ei voi muuttaa.

**V5 Ohjaimen fonttikoko - Rivimäärä:**

* Standardi Fontti - 3 riviä (oletus)

![controller_screen_info](v5_controller_rows_columns.jpg)

<advanced>
</advanced>
