category: sensing  
signature: brain.screen.row()  
description: Reports the row number of the V5 Brain screen cursor location.

# Kursorin rivi aivojen näytöllä

Antaa kursorin rivinumeron aivojen näytöllä.

```don
brain.screen.row()
```

## Miten käytetään

Näytön rivien lukumäärä oletusfontilla on välillä **1 to 20**.

Voit muuttaa fontin kokoa näytöllä ja samalla se vaikuttaa rivien määrään:

**V5 Aivojen fonttikoko - Rivien määrä:**

* `FontType.MONO12` - 20 Riviä
* `FontType.MONO15` - 16 Riviä
* `FontType.MONO20` / `FontType.PROP20` - 12Riviä (Oletus)
* `FontType.MONO30` / `FontType.PROP30` - 8 Riviä
* `FontType.MONO40` / `FontType.PROP40` - 6 Riviä
* `FontType.MONO60` / `FontType.PROP60` - 4 Riviä
	
<advanced>
</advanced>
