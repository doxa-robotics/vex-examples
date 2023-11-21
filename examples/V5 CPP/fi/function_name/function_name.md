category: functions  
signature: function_name
device_class: function  
description: Runs the specified function when the bumper is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Funktiot

Funktiot on joukko komentoja/koodinippuja , jotka suorittavat jonkin määrätyn tehtävän.

```don
def my_function():
    pass
```
## Miten käytetään

Kun luot funktion anna sille kuvaava nimi, joka kuvaa sen toimintaa.

Määrittele, mitä muotoa tietoa olevaa tietoa se palauttaa. Muodot - `int`, `float`, `double`, ja `string` ovat tyypillisimmät. Jos funktio ei palauta , määrittele se muotoa `void`.

Sisällytä sulut `()` lisä *parametreille* funtionimen jälkeen. Useampi parametri erotellaan pilkulla (parameter1, parameter2).

Funktion runko kirjoitetaan aaltosulkujen `{ }` sisään.

```cpp
int returnZero() {
  return 0;
}
```

## Esimerkki 

Tällä 'void' funktiolla ei ole parametreja ja se tulostaa "The battery is low!" V5 Aivojen näytölle.


```cpp
void lowOnBattery() {
  if (Brain.Battery.capacity() < 25.0) {
    Brain.Screen.print("The battery is low!");
  }
}
```
```

<advanced>
</advanced>