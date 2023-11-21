category: sensing  
signature: inertial.gyro_rate(AxisType.XAXIS, VelocityUnits.DPS)
description:  Gets the rate of rotation from one of the axes (x, y, or z) on the Inertial Sensor.

# Inertia -sensorin kääntymisnopeus

Antaa kääntymisnopeuden yhdeltä akselilta (x, y, tai z).

```don
inertial.gyro_rate(AxisType.XAXIS, VelocityUnits.DPS)
```

## Miten käytetään

Inertia -sensorin kääntymisnopeus antaa arvot välillä **-1000.0 - 1000.0** yksikkönä dps (astetta sekunnissa).

Valise akseli, jota tarkastelet. Valinnat ovat:

* X-akseli raportoi kääntymisnopeuden x-akselilla
* Y-akseli raportoi kääntymisnopeuden y-akselilla
* Z-akseli raportoi kääntymisnopeuden z-akselilla


<advanced>
</advanced>
