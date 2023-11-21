category: drive  
signature: drivetrain.drive(FOWARD)  
description: Moves the Drivetrain forever in the direction specified inside of the parentheses. 

# Aja

Ajopeli liikkuu ikuisuuden suuntaan, joka määritelty suluissa. 

Kaikki ajopelin ajomoottorit ajavat eteen tai taaksepäin nopeutta , joka on määritelty komennolla `drivetrain.set_drive_velocity`, oletus on 50%. 

Negatiiviset nopeusarvot aiheuttavat sen, etttä ajopeli ajaa vastakkaiseen suuntaan parametrilla  FORWARD .

```don
drivetrain.drive(DIRECTION)
```

## Miten käytetään

`drivetrain.drive` komennolla ajopeli ajaa ikuisuuden, kunnes joku uusi ajokomento on annettu tai ohjelma on lopetettu.

## Esimerkit

Käytä `FORWARD` argumenttia isoilla kirjaimilla, kun ajopeli ajaa eteenpäin

```don
drivetrain.drive(FORWARD)
```

Käytä `REVERSE` argumenttia isoilla kirjaimilla, kun ajopeli peruuttaa


```don
drivetrain.drive(REVERSE)
```
 
<advanced>
</advanced>
