category: sensing  
signature: Drivetrain.efficiency(percent)  
device_class: drivetrain  
description: Reports the efficiency of the Drivetrain.

# Ajopelin tehosuhde/hyötysuhde

Antaa ajopelin tehosuhteen.

```cpp
Drivetrain.efficiency()
```

## Miten käytetään

`Drivetrain.efficiency()` antaa suhteen ajopelin ajomoottoreiden ulostuhoteho (output) watteina suhteessa sisääntulo (input) tehoon watteina 

V5 ajopeli saavuttaa tyypillisesti 65% hyötysuhteen.


`Drivetrain.efficiency()` antaa desimaaliluvun (muotoa *double*) yksikkönä `percent` (%) ja arvon välillä  **0.0% - 100.0%**.

```cpp
Brain.Screen.print("%f", Drivetrain.efficiency());
```
<advanced>
</advanced>