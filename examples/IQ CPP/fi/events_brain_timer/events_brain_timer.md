category: events  
signature: events_brain_timer
description: Runs the specified function when the IQ Brain's timer is greater than the given value.

# Kello tapahtuma

Tehdään callback joka suoritetaan tietyna jan kuluttua.

```cpp
Brain.Timer.event(callback, time);
```

## Miten käytetään

IQ Aivojen kello käynnistuu ohjelman alussa.

`Brain.Timer.event` funktioon annetaan 2 parametria.

Ensimmäinen on ns **callback funktio** parametri. Funtio pitää luoda/nimetä, jotta se voidan välittää `Brain.Timer.event` funktion parametrina.

Toinen parametri on aika. jolloin funktio suoritus alkaa. **Callback funkktion** koodi alkaa pyörimään heti kun **Brain Timer** aikamäärä on suurempi kuin parametrin arvo `time` yksikössä **millisekuntia**.

```cpp
// Call the callback function after 1000 milliseconds
Brain.Timer.event(callback, 1000);
```

## Callback Funktiot

Callback funktion on käyttäjän määrittämä funktio, joka välitetään argumenttina tosielle funktiolle. **Callback funktion** koodi suoritetaan kun ko tapahtuma **event** sattuu.

Esimerkissä "Callback Function Called" teksti tulostetaan  VEX IQ's Aivojen näytölle 10 sekunnin kuluttua ohjelma alusta.

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Brain.Timer.event(callbackFunction, 10000);
}
```

<advanced>
</advanced>