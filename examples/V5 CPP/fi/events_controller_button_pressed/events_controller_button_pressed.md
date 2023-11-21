category: events  
signature: CONTROLLER.BUTTON.pressed(callback);  
device_class: controller  
description: Runs the specified function when the controller button is pressed.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Ohjaimen nappia painettu

Suorittaa tietyn funktion kun Ohjaimen tiettyä nappia on painettu.

```cpp
Controller1.ButtonA.pressed(callback);
```


## Miten käytetään

Valitse ohjaimen nappi (kts ohjaimesta merkinnät napeille).

* `ButtonA`
* `ButtonB`
* `ButtonX`
* `ButtonY`
* `ButtonUp`
* `ButtonDown`
* `ButtonLeft`
* `ButtonRight`
* `ButtonL1`
* `ButtonL2`
* `ButtonR1`
* `ButtonR2`

Luo funktio , jota kutsutaan kun ohjaimen ko. nappia on painetttu. 

Anna funktiolle nimi, joka välitetään kutsuparametrissa, kun funktion toiminta suoritetaan nappia painettaessa.

```cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  Controller1.ButtonA.pressed(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```



<advanced>
</advanced>