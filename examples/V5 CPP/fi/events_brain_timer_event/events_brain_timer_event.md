category: events  
signature: Brain.Timer.event(callback, 1000);  
description: Runs the specified function when the V5 Brain's timer is greater than the given value.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Aivojen kello tapahtuma

Suorittaa halutun callback -funktion, kun V5 Aivojen kello on suurempi kuin annettu parametriarvo.

```cpp
Brain.Timer.event(callback, 1000);
```

## Miten käytetään

V5 Aivojen kello käynnistyy ohjelman alussa.

Määritä aikaraja tapahtumalle. `Brain.Timer.event();` tapahtuma suoritetaan kerran, kun kello on **suurempi kuin** annettu aikaraja.

`Brain.Timer.event();` hyväskyy kokonaislukuja ja yksikkönä on millisekunnit.

Luo funktio , jota kutsutaan, kun kello on käynyt yli aikarajan. Nimeä funktio ja käytä sitä tapahtuman `callback` parametrina.

```cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  Brain.Timer.event(runOnEvent, 2000);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```


<advanced>
</advanced>