category: sensing  
signature: MOTOR.direction()  
device_class: motor  
description: Reports the direction a V5 Smart Motor is currently spinning.

# Motor.direction()

Antaa suunnan, johon V5 älymoottori pyörii tällä hetkellä.

```cpp
Motor.direction()
```

## Miten käytetään

Komennot jotja antavat arvon voidaan käyttää muiden komentojen sisällä mm print -komennossa tai toistorakenteiden ehtolauseissa (ilman puolipistettä rivin lopussa).

`Motor.current()` palauttaa **directionType** arvon, joka voi olla joko `forward` (eteenpäin) tai `reverse` (taaksepäin).


```cpp
if (LeftMotor.direction() == forward) {
    Brain.Screen.print("Left Motor is spinning forward!");
}
```
**Note:** Puolipistettä käyttää yllä `print` -komento.
<advanced>
</advanced>