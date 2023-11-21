category: variables  
signature: variables_boolean
description: Declares the type, name, and value of a Boolean. 

# Boolean Muuttuja

Muuttaja saa arvot **tosi** tai **epätosi**.

`bool myBoolean = true;`

## Miten käytetään

**Boolean Muuttuja** arvo voi olla **tosi** tai **epätosi**. Määrittele muuttujanimen alkuun `bool` ja anna sille alkuarvo `tosi` tai `epätosi`. 

`bool goFast = true;`

Boolean muuttujia voi käyttää ohjauskomentojen ehdoissa. 

```cpp
if (goFast) {
  Drivetrain.setDriveVelocity(100, percent);
}
```

<advanced>
</advanced>