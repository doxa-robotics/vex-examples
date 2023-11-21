category: functions  
signature: function_name
device_class: function  
description: Runs the specified function when the bumper is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Funktiot

Funktioiksi kutsutaan joukkoa komentoja , jotka voi suorittaan useampaan kertaan kutsuttaessa.

```cpp
void myFunction() {
  // function code
}
```

## Miten käytetään

Määrittele funktio ja määritä datatyyppi, jonka funtio palauttaa.

- `int` (kokonaisluku), `float` (liukuluku), `double` (desimaaliluku), ja `string` (merkkijoino) ovat datatyypit normaalisti. Jos funtio ei palauta mitään arvoa, määrittele se tyypiksi `void`. 

Kannataa määritellä funktion nimi kuvaavaksi, mitä se tekee.

```cpp
int returnZero() {
  return 0;
}
```

Kutsuparametrit *parameters* laitetaan sulkuihin `()`funtionimen jälkeen. Useampi parametri erotellaan pilkuilla (parameter1, parameter2).

Funktion komennot laietaan aaltosulkuihin `{ }`.
    
## Esimerkki

Tämä fuktio ei palauta arvoa ts se on tyyppiä `void`. Se tulostaa "The battery is low!" VEX IQ Aivojen näytölle, kun akun varaustaso on alle 25%.

```cpp
void lowOnBattery() {
  if (Brain.Battery.capacity(percent) < 25.0) {
    Brain.Screen.print("The battery is low!");
  }
}
```

<advanced>
</advanced>