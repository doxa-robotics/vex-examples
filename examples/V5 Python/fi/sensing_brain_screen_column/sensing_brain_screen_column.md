category: sensing  
signature: brain.screen.column()  
description: Reports the column number of the V5 Brain screen cursor location.

# Näytön Kursorin sarake

Antaa V5 Aivojen näytöllä kursorin paikan.

```don
brain.screen.column()
```

## Miten käytetään

Näytön sarake voi olla välillä **1 - 80**.

V5 Aivojen näytöklle voi määritellä fontin kokoa ja samaal se vaikuttaa sarakkeiden määrään.

**V5 Aivojen fonttikokoe - Sarakkeiden määrä:**

* `FontType.MONO12` - 80 saraketta
* `FontType.MONO15` - 68 saraketta
* `FontType.MONO20` / `FontType.PROP20` - 48 saraketta (Oletus)
* `FontType.MONO30` / `FontType.PROP30` - 32 saraketta
* `FontType.MONO40` / `FontType.PROP40` - 24 saraketta
* `FontType.MONO60` / `FontType.MONO60` - 16 saraketta
	
<advanced>
</advanced>
