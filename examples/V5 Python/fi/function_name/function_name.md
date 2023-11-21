category: functions  
signature: def function_name(parameters):\n\tpass  
description: Functions are blocks of code used to perform an action.

# Funktiot

Funktiot on joukko komentoja/koodinippuja , jotka suorittavat jonkin määrätyn tehtävän.

## Miten käytetään

Kun luot funktion, anna sille kuvaava nimi, joka kuvaa sen toimintaa.

Käytä **keyword** (avainsana) `def` ennen funktion nimeä, kun määrittelet funktion.

Sisällytä parametrit funktion nimen jälkeen sulkuihin `()` ja loppuun kaksoispiste `:`.Jos parametreja on useampi, niin laita ne pilkulla erottaen sulkujen sisään `(parameter1, parameter2)`.

Funktion runkoon komennot sisennetään 4 tyhjällä merkillä. Jos komentoja ei o0le, lisää kuitenkin sana `pass` komentoriville.

```don
def my_function():
    pass
```

## Esimerkki 1

Tällä funktiolla ei ole parametreja ja se tulostaa sanan "Hello" V5 Aivojen näytölle.

```don
def print_hello_world():
    brain.screen.print("Hello World")
```
## Esimerkki 2

Tässä funktiossa on 1 paremetri `name` se tulostaa `name` muuttujan nimen V5 Aivojen näytölle.

```don
def print_name(name):
    brain.screen.print(name)
```

<advanced>
</advanced>
