category: drivetrain 
signature: drivetrain.turn(RIGHT)  
description: Turns the Drivetrain to the right or left.  

# Käänny

Ajopeli kääntyy jatkuvasti joko oikealle tai vasemmalle.

```don
drivetrain.turn(DIRECTION)
```

## Miten käytetään

`drivetrain.turn` komennolla ajopeli kääntyy ikuisesti haluttuun suuntaan kunnes joku uusi komento sen kumoaa tai ohjelma loppuu.

Käytä `LEFT` argumenttia isoilla kirjaimilla, kun käännät vasemmalle.

```don
drivetrain.turn(LEFT)
```

Käytä `RIGHT` argumenttia isoilla kirjaimilla, kun käännät oikealle.

```don
drivetrain.turn(RIGHT)
```

## Esimerkki

Esimerkissä ajopelia ajaa eteenpäin 200 MM ennen kuin kääntyy oikealle ikuisuuden.

```don
drivetrain.drive_for(FORWARD, 200, MM)

drivetrain.turn(RIGHT)
```

<advanced>
</advanced>
