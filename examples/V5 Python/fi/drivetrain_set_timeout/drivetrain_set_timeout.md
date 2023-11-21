category: drivetrain
signature: drivetrain.set_timeout(TIME, SECONDS)
description: Sets a time limit for the robot movement commands.

# Aseta aikaraja

`drivetrain.set_timeout(TIME, SECONDS)` asettaa aikarajan, kuinka kauan robotin liikekomento jatkuu.

## Miten käytetään

Komentoa käytetään estämään ohjelman keskeytys jos seuraava liikekomento ei pääse tavoiteasemaan.

Aseta määrä sekunteina `SECONDS`.

## Esimerkki

Esimerkissä on asetettu 3 sekunnin aikaraja ajo komennolle.

```don
drivetrain.set_timeout(3, SECONDS)
drivetrain.drive_for(FORWARD, 1000, MM)
```

<advanced>
</advanced>
