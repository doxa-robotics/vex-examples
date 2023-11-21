category: sensing  
signature: Motor.current(units)  
device_class: motor  
description: Reports the amount of current a Motor is currently using.

# Moottorin sähkövirta

raportoi määrän, jota VEX IQ älymoottori kuluttaa sähköä tällä hetkellä.

```cpp
Motor.current(units)
```

## Miten käytetään

`Motor.current` palauttaa desimaaliluvun (muoto *double*) ja antaa sähkövirran kulutustiedon, jota moottori tällä hetkellä kuluttaa.

`Motor.current` komento hyväkyy sekä **amp** (Ampeeria) or **percent** as a valid `units` parameter.

Tulostetaan sähkövirta prosentteina:

```cpp
Brain.Screen.print("%f" , Motor.current(percent));
```

Tulostetaan sähkövirta ampeereina:

```cpp
Brain.Screen.print("%f", Motor.current(amp));
```

<advanced>
</advanced>