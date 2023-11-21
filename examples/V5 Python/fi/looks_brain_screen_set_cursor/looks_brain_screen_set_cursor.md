category: looks  
signature: brain.screen.set_cursor(1, 1)
description: Sets the cursor location for brain.screen.print() command on the V5 Brain's screen.

# Aseta kursorin paikka


Asettaa kursorin V5 Aivojen näytöllä.

```don
brain.screen.set_cursor(ROW, COLUMN)
```

## Miten käytetään

Komento `brain.screen.set_cursor()` vaatii kaksi arvoa:

* Arvo 1: Näytön rivinumero 
* Arvo 2: Näytön sarakenumero 

`brain.screen.print()` komennolla kursori haluttuun kohtaan näyttöä.

Rivin  **row** voi valita väliltä **1 - 20**.

Sarakkeen **column** voi valita väliltä **1 - 80**.

---

V5 Aivoille tulstettaessa voit valita kirjaisnlajin ja koon. Valinnat vaikuttavat, kuinka monta riviä ja saraketta näytölle mahtuu seuraavasti:

**V5 Aivojen fontin koko - Rivien määrä:**

* `FontType.MONO12` - 20 riviä
* `FontType.MONO15` - 16 riviä
* `FontType.MONO20` / `FontType.PROP20` - 12 riviä (Oletus)
* `FontType.MONO30` / `FontType.PROP30` - 8 riviä
* `FontType.MONO40` / `FontType.PROP40` - 6 riviä
* `FontType.MONO60` / `FontType.PROP60` - 4 riviä

**V5 Aivojen fontin koko - Sarakkeiden määrä:**

* `FontType.MONO12` - 80 saraketta
* `FontType.MONO15` - 68 saraketta
* `FontType.MONO20` / `FontType.PROP20` - 48 saraketta (Oletus)
* `FontType.MONO30` / `FontType.PROP30` - 32 saraketta
* `FontType.MONO40` / `FontType.PROP40` - 24 saraketta
* `FontType.MONO60` / `FontType.MONO60` - 16 saraketta

![brain_screen_info](v5_row_column_brain.jpg)

<advanced>
</advanced>
