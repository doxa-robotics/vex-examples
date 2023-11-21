category: drivetrain
signature: Drivetrain.setDriveVelocity(50, percent);  
device_class: drivetrain  
description: Sets the velocity of the Drivetrain that will be used for drive and driveFor calls. If this is used when the drive is moving, the drivetrain will be updated with the new speed. 

# Aseta ajopelin nopeus

Asettaa ajopelin nopeuden, jota käytetään `Drivetrain.drive` ja `Drivetrain.driveFor` komennoissa. 

Jos komentoa käytetään ajopelin ajon aikana, niin nopeus päivittyy uudeksi nopeudeksi kesken ajon.

```cpp
Drivetrain.setDriveVelocity(velocity, units);
```

## Miten käytetään

`Drivetrain.setDriveVelocity` asettaa ajopelin nopeuden, mutta ei liikuta sitä.

`Drivetrain.setDriveVelocity` hyväksyy arvot väliltä **-100 - 100**, kun käytetään yksikköä **percent** (prosenttia).

`Drivetrain.setDriveVelocity` hyväksyy arvot väliltä **-127 - 127**, kun käytetään yksikköä **rpm** (kierrosta minuutissa).

Jos ajopelin nopeudeksi asetetaan negatiivinen luku, ajopeli liikkuu taaksepäin oletuksesta.

Jos ajopelin nopeudeksi asetetaan nolla, ajopeli pysähtyy.

## Example

Esimerkissä ajopelin nopeudeksi asetetaan 50 % ja ajetaan sillä matka 12 tuumaa.

```cpp
Drivetrain.setDriveVelocity(50, percent);
Drivetrain.driveFor(forward, 12.0, inches);
```

<advanced>
</advanced>
