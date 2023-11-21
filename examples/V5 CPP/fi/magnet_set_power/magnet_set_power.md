category: magnet  
signature: MAGNET.setPower(100);  
device_class: electromagnet  
description: Sets the power of a V5 Electromagnet that will be used when picking up a magnetic object  

# Aseta sähkömagneetin voima

Muuttaa sähkömagneetin tarttumiskykyvoimaa

```cpp
Magnet.setPower(power);
```

Voimaa voi säätää välillä **0% - 100%**.

## Esimerkki

Esimerkissä `magnet.set_power()` komennolla asetetaan täsyi 100 % teho, pomitaan esine , ajetaan eteenpäin ja pudotetaan esine.

```cpp
Magnet.setPower(100);
Magnet.pickup();
```

<advanced>
</advanced>






