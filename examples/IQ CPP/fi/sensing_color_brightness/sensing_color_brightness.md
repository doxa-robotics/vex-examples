category: sensing  
signature: Color.brightness()  
description: Reports if a button on the VEX IQ Brain is pressed.

# Värin valovoima %

Raportoi värisensorin havaitseman värin valovoiman/kirkkauden.

```cpp
Color.brightness()
```

## How To Use

`Color.brightness` raportoi arvot väliltä **0% - 100%**.

Komennon ensimmäinen osa on nimetty värisensori.

```cpp
Color2.brightness()
Color4.brightness()
```

Mitä enemmän valoa sitä suurempi arvo, mitä himmeämpi valo sitä pienempi arvo.

## Esimerkki

Esimerkissä tulostetaan värisensorin havaitseman valon kirkkaus/valovoima.

```cpp
Brain.Screen.print("Brightness: %d", Color.brightness());
```

<advanced>
</advanced>
