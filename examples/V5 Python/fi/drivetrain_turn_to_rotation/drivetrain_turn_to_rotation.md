category: drivetrain
signature: drivetrain.turn_to_rotation(90, DEGREES, wait=True)
description: Turns the Drivetrain to a specific angle of rotation..  

# Käännä kiertokulmaa määrän

Kääntää ajopeliä kiertokulman tiettyyn astemäärään nykyisen gyron astemäärän perusteella.

`drivetrain.turn_to_rotation(ROTATION, DEGREES)`

## Miten käytetään

drivetrain.turn_to_rotation` komentoa voi käyttää kääntämään ajopeliä positiivisen arvolla myötäpäivään tai negatiivisella arvolla vastapäivään.

Riippuen nykyisestä kääntymiskulman arvosta gyrosensorissa `drivetrain.turn_to_rotation` päättelee mihin suuntaan se kääntyy.

`ROTATION` parametri hyväksyy numeerisia rvoja.

Numeeriset arvot eivät **not** rajoita arvoja välillä **0 - 359.99** astetta. Käännökset ovat absoluuttisia ja voivat kääntää robottia enemmän kuin kerran

## Esimerkki

Esimerkissä ajopeli tekee 4 käännöstä:

```don
drivetrain.turn_to_rotation(90.0, DEGREES)
drivetrain.turn_to_rotation(180, DEGREES)
drivetrain.turn_to_rotation(-45, DEGREES)
drivetrain.turn_to_rotation(0, DEGREES)
```

- Oikealla myötäpäivään kohtaan 90 astetta
- Oikealla myötäpäivään kohtaan 180 astetta
- Vasemmalle vastapäivään kohtaan -45 astetta
- Oikealla myötäpäivään kohtaan 0 astetta

'drivetrain.turn_to_rotation` komento estää muiden komentojen suorituksen , jos käännös on kesken.

## Lisäparametri 

Voit lisätä lisäparametrin `wait=False`, jolloin `turn_to_rotation` komento ei estä seuraavien komentojen suoritusta kesken käännöstä.

```don
drivetrain.turn_to_rotation(180.0, DEGREES, wait=False)
```

<advanced>
</advanced>
