category: magnet  
signature: magnet.set_power(50)
description: Changes the power used by the V5 Electromagnet when picking up objects.

# Aseta sähkömagneetin voima

Muuttaa sähkömagneetin tarttumiskykyvoimaa

```
magnet.set_power(50)
```
Voimaa voi säätää välillä **0% - 100%**.

## Esimerkki

Esimerkissä `magnet.set_power()` komennolla asetetaan täsyi 100 % teho, pomitaan esine , ajetaan eteenpäin ja pudotetaan esine.

```
magnet.set_power(100)
magnet.pickup()
drivetrain.drive_for(FORWARD, 200, MM)
magnet.drop()
```

<advanced>
</advanced>