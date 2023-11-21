category: sensing  
signature: Color.detects(color)  
device-class: colorsensor
description: Reports if a color sensor detects a specific color.

# Värisensori havaitsee tietyn värin?

Raportoi värin nimen, jonka värisensori havaitsee.

```cpp
Color.detects(color)
```

## Miten käytetään

Raportoi arvon **tosi** kun värisensori havaitsee tietyn värin ja  **epätosi** kun ao väriä ei havaita.

Komennon alku on nimetty värisensori.

```cpp
Color1.detects(red)
Color2.detects(blue)
```

Valitse väri, jonka värisensori havaitsee.

- `punainen`
- `oranssi`
- `keltainen`
- `vihreä`
- `sininen`
- `punavioletti`
- `violetti`
- `puna-violetti`
- `sini_violetti`
- `sini-vihreä`
- `kelta-vihreä`
- `kelta-oranssi`
- `puna-oranssi`
- `valkoinen`

Voit myös valita **colorType::none** jos värisensori **ei** havaitse esinettä.

## Esimerkki

TTässä esimerkissä tulostetaan joko "Color Red" , jos värisensori havaitsee punaisen esineen tai "Other Color" jos punaista ei havaita.

```cpp
if (Color.detects(red)) { 
  Brain.Screen.print("Color Red");
} else {
  Brain.Screen.print("Other Color");
}
```

<advanced>
</advanced>