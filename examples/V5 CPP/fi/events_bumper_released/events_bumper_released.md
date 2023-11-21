category: events  
signature: BUMPER.released(callback);  
device_class: bumper  
description: Runs the specified function when the bumper is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

## Painokytkin vapautettu

Suorittaa halutun funktion kun painokytkin vapautetaan

```cpp
BumperA.released(callback);
```


## Miten käytetään

Luo funktio, jota kutsutaan, kun painokytkin on vapautettu. 

Anna funktiolle nimi ja toiminnot. Nimi välitetään callback - parametrina kun painokytkin on vapautettu.

``cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  BumperA.released(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>