category: control  
signature: else { }  
description: Runs the code inside the else-statement's curly brackets, if the if-statement's condition is false. This command must have an if-statement preceding for it to compile.  

# Jos/muuten

Ohjauslause, joka suorittaa If -haaran, jos ehto on 'true' (tosi) ja Else -haaran jos ehto on 'false' (epätosi).

```cpp
if (condition) {

} else {

}
```

## Miten käytetään

'if` komento on ehto , joka saa joko arvon **True** tai **False**. Voit yhdistää ehtoihin useamman loogisen operaattorin `and`, `or`, and `not`. 

Jos ehto saa arvon **True**, `if ehdon` haaran komennot aaltosuluissa suoritetaan. Jos ehto saa arvon **False**, `else:` haaran komennot aaltosuluissa suoritetaan.

```cpp
if (BumperA.pressing()) {
    LeftMotor.stop();
} else {
    LeftMotor.spin(forward);
}
```

<advanced>
</advanced>