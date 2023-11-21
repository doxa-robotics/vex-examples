category: events  
signature: BUMPER.pressed(callback);  
device_class: bumper  
description: Runs the specified function when the bumper is pressed.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Painokytkintä painettu

Suorittaa halutun funktion kun painokytkintä painettu.

```cpp
BumperA.pressed(callback);
```

## Miten käytetään

Luo funktio, jota kutsutaan, kun painokytkintä on painettu. 

Anna funktiolle nimi ja toiminnot. Nimi välitetään callback - parametrina kun painokytkintä on painettu.

```cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  BumperA.pressed(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```

`
<advanced>
</advanced>