category: motion  
signature: Motor.spinFor(forward, 90, degrees);  
device_class: Motor  
description: Spins the motor for a number of degrees or turns.  

# Pyöritä moottoria määrän

Pyörittää VEX IQ Älymoottoria tietyn asetetun määrän yksiköitä.

```cpp
Motor.spinFor(direction, rotation, units);
```

## Miten käytetään

`Motor.spinFor` pyörittää VEX IQ Älymoottoria asetettuun suuntaan asetetun määrän yksiköitä .

Mahdolliset argumentit:

- `direction` (suunta) hyväksyy joko arvon **forward** (eteenpäin) tai arvon **reverse** (taaksepäin)
- `rotation` (kierroksia) hyväksyy numeeerisen arvon
- `units` (yksikkö) hyväksyy joko **degrees** (asteita) tai **turns** (kierroksia)

`Motor.spinFor` estää muiden komentojen suorituksen kunnes sen liike on päättynyt.

## Lisäparametrit

Voit asettaa lisäparametrin `false` (epätosi) viimeiseksi parametriksi, jos haluet ettei `Motor.spinFor` komennon suoritus estä seuraavien komentojen suoritusta .

```cpp
Motor.spinFor(reverse, 360, degrees, false);
```

<advanced>
</advanced>
