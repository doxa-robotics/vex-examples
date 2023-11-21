category: sensing  
signature: inertial.orientation(OrientationType.ROLL , DEGREES)
description:  Gets an orientation angle of the inertial sensor. Reports the unit value specified by the parameter of the inertial sensor.

# Inertial suunta

Antaa inertial sensorin mittaaman suuntakulman. Tulos annetaan sille suunnalle (x,y tai z) , jonka parametri käytössä.

```don
inertial.orientation(OrientationType.ROLL, DEGREES)
```

## Miten käytetään

Tulos annetaan sille suunnalle (x,y tai z).

* X-akseli edustaa pitch (eteen-taakse) välillä -90 - +90 astetta.
* Y-akseli edustaa roll (sivulta-sivulle) välillä -180 - +180 astetta
* Z-aakseli edustaa yaw (ylös-alas) välillä  -180 - +180 astetta

<advanced>
</advanced>
