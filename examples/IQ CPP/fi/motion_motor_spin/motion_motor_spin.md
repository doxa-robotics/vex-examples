category: motion  
signature: Motor.spin(forward);  
device_class: motor  
description: Spins a Motor in a direction until stopped.  

# Pyöritä Moottoria

Pyörittää VEX IQ Älämoottoria haluttuun suuntaan (kunnes se pysäytetään).

```cpp
Motor.spin(direction);
```

## Miten käytetään

`Motor.spin` komento pyörittää VEX IQ Älymoottora ikuisesti kunnes uusi moottorikomento on annettu tai ohjelman suoritus loppuu.

- **forward** pyörittää moottoria eteenpäin
- **reverse** pyörittää moottoria taaksepäin

```cpp
Motor.spin(forward);
Motor.spin(reverse);
```

<advanced>
</advanced>