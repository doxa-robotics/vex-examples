category: events  
signature: CONTROLLER.AXIS.changed(callback);  
device_class: controller  
description: Runs the specified function when the controller axis value changes.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Ohjaimen tatin asentoa muutettu

Suorittaa määrätyn funktion, kun ohjaimen tatin asentoa muutettu.

```cpp
Controller1.Axis1.changed(callback);
```

## Miten käytetään

Valitse ohjaimen tatti, jota käsitellään.

* `Axis1`
* `Axis2`
* `Axis3`
* `Axis4`

Luo funktio ohjaimen tatille , joka käsittelee tatin käyttöä. 

Anna funktiolle nimi, jota käytetään `callback` parametrissa, kun tatin asentoa on muutettu kutsuttaessa itse funktiota.

`
```cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  Controller1.Axis1.changed(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>