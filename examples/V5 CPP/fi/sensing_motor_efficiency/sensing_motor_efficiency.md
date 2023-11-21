category: sensing  
signature: MOTOR.efficiency(percent)  
device_class: motor  
description: Reports the efficiency of the V5 Smart Motor.

# Moottorin tehokkuus

Antaa V5 Älymoottorin suhteellisen tehokkuuden/hyötysuhteen.

```cpp
Motor.efficiency(percent)
```

## Miten käytetään

`Motor.efficiency()` raportoi moottorin ulostulotehon output (W) suhteen sisääntulotehoon input (W). 

V5 Älymoottori tyypillisesti pääsee maksimissaan 65% hyötysuhteeseen normaaliolosuhteissa.

Komentoja, jotka antavat tämäntyyppisiä arvoja, käytetään muitten kuten print komentojen parametreissa tai toistorakenteiden ehdoissa.

`Motor.efficiency()` antaa desimaalilukuarvoja (kuten *double*) yksikkönä `percent` (%) arvoväliltä **0.0% - 100.0%**.

```cpp
Brain.Screen.print("%f", Motor.efficiency(percent));
```
<advanced>
</advanced>
