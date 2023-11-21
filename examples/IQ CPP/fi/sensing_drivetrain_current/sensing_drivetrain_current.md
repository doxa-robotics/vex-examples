category: sensing  
signature: Drivetrain.current(units)  
device_class: drivetrain  
description: Reports the amount of current (power) that the Drivetrain is currently using.

# Ajopelin sähkövirta

Raportoi ajopelin virrankulutuksen tällä hetkellä.

```cpp
Drivetrain.current(units)
```

## Miten käytetään

`Drivetrain.current` palauttaa desimaalilukuarvon (*double*) , kun raportoidaan ajopelin tämänhetkistä virrankulutusta.

`Drivetrain.current` palauttaa valitun `yksikkö` mukaisen arvon.

Valittavaissa on yksiköt **amp** (ampeerit) or **prosentti**.

## Esimerkki

Esimerkissä tulostetaan ajopelin asähkövirta yksikössä amp (ampeeri) VEX IQ robotin aivojen näytölle.

```cpp
Brain.Screen.print("%f", Drivetrain.current(amp));
```

<advanced>
</advanced>