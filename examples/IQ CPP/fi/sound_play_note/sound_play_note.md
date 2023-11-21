category: sound 
signature: Brain.playNote(octave, note, duration);  
device_class: sound  
description: Plays the selected musical note.

# Soita Nuotti

Soittaa valitun musiikkinuotin.

```cpp
Brain.playNote(octave, note, duration);
```

## Miten käytetään

Valitse oktaavi, alhaisin on 1 ja korkein on 7. 

Valitse seuraavaksi oktaavin nuotti, joka soitetaan:
- `C = 0`
- `D = 1`
- `E = 2`
- `F = 3`
- `G = 4`
- `A = 5`
- `B = 6`

Valise kesto nuotille **millisekunteina**:

- Koko nuotti 1 s (1000 ms)
- Puoli nuotti 0.5 s (500 ms)
- Neljännes nuotti 0.25 s (250 ms)

Heti kun nuotin soitto alkaa, suoritetaan myös seuraava komento ohjelmassa.

## Esimerkki

Tämä soittaa keskipktaavin C kokonuotin 1 s ajan.

```cpp
Brain.playNote(4, 0, 1000);
```

<advanced>
</advanced>