category: drive  
signature: Drivetrain.turn(right);  
device_class: drivetrain  
description: Turns the Drivetrain.  

# Käänny

Ajopeli kääntyy jatkuvasti joko oikealle tai vasemmalle.


```cpp
Drivetrain.turn(turnType);
```


## Miten käytetään

`Drivetrain.turn();`  komennolla ajopeli kääntyy ikuisesti haluttuun suuntaan kunnes joku uusi komento sen kumoaa tai ohjelma loppuu.

Käytä `LEFT` argumenttia isoilla kirjaimilla, kun käännät vasemmalle.

```cpp
Drivetrain.turn(left);
```

Käytä `RIGHT` argumenttia isoilla kirjaimilla, kun käännät oikealle.

```cpp
Drivetrain.turn(right);
```

<advanced>
</advanced>