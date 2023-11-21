category: drivetrain  
signature: drivetrain.stop()  
description: Stops the Drivetrain.  

# Pysäytä

Pysäytä ajopeli.

```don
drivetrain.stop()
```

## Miten käytetään

`drivetrain.stop()` komento pysäyttää ajopelin. Sillä ei ole argumentteja.

## Esimerkki

Esimerkissä ajopeli pysähtyy kun se on ajanut 3 sekuntia eeenpäin.

```don
drivetrain.drive(FORWARD)
wait(3, SECONDS)
drivetrain.stop()
```

<advanced>
</advanced>
