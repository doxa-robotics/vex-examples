category: drive  
signature: Drivetrain.stop();  
device_class: drivetrain  
description: Stops the Drivetrain.  

# Pysähdy

Pysäyttää ajopelin.

```cpp
Drivetrain.stop();
```

## Miten käytetään

`Drivetrain.stop` komento pysäyttää ajopelin.

Pysähtymistavan voi asettaa `Drivetrain.setStopping` komennolla.

## Esimerkki

Esimerkissä VEX IQ robotti liikkuu eteenpäin 3 sekuntia ja sen jälkeen pysähtyy.

```cpp
Drivetrain.drive(forward);
wait(3, seconds);
Drivetrain.stop();
```

<advanced>
</advanced>