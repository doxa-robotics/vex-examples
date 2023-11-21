category: sensing  
signature: ACCEL.acceleration()  
device_class: accelerometer  
description: Reports the acceleration value from one axis on the Analog Accelerometer.

# Kiihtyvyysmittarin kiihtyvyys

Antaa analogisen kiihtyvyysmittarin kiihtyvyysarvon akseleilla (x, y, or z).

X-akselin suuntaan saadaan horisontaalinen kiihtyvyysarvo ja Y-akselilla vertikaalinen . Z-akselilla saadaan kiihtyvyys ylöspäin.

```cpp
Accel2G.acceleration()
```

## Miten käytetään


`Accelerometer.acceleration()` antaa desimaaliluvun (muotoa *double*) välillä **-2.0 G - 2.0 G** tai **-6.0 G - 6.0 G** riipuen laitteen jumpperiasetuksista.

1.0 G vastaa arvoa 9.8 metriä sekunnin toisessa potenssissa.

```cpp
Brain.Screen.print("%f", Accel2GB.acceleration());
```
<advanced>
</advanced>