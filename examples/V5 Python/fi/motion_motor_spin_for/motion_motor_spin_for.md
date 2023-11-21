category: motion  
signature: motor.spin_for(FORWARD, 90, DEGREES)  
description: Spins a V5 Smart Motor for a given distance.

# Pyöri matka
 
Komento pyörittää V5 älymoottoria tietyn matkan joko asteina tai kierroksina.

```don
motor.spin_for(DIRECTION, AMOUNT, UNIT)
```

## Miten käytetään

Valitse suunta `DIRECTION` , johon moottori pyörii: **FORWARD** (eteenpäin) tai **REVERSE** (taaksepäin).

Valitse mittayksikkö `UNIT` joko **DEGREES** (%) tai **TURNS** (kierroksia).

Valitse odottaako seurava kometo pyörimisen loppuun joko **wait=True** (odota) tai **wait=False** (jatka seuraavaan komentoon heti). 

```don
motor.spin_for(FORWARD, 90, DEGREES, wait=False)
```

Oletuksena on aina odotus ellei parametria **wait=False** ole erikseen annettu.

<advanced>
</advanced>
