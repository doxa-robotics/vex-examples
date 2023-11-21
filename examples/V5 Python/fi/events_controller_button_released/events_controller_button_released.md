category: events  
signature: controller.button.released(callback)  
device_class: controller  
description: Runs the specified function when the controller button is released.  

# Ohjaimen nappi vapautettu

Suorittaa haluton funktion komennot kun ohjaimen nappi vapautetaan.

```python
controller.button.released(callback)
```

## Miten käytetään

Valitse ohjaimen nappi, jota käytät.

* `buttonA`
* `buttonB`
* `buttonX`
* `buttonY`
* `buttonUp`
* `buttonDown`
* `buttonLeft`
* `buttonRight`
* `buttonL1`
* `buttonL2`
* `buttonR1`
* `buttonR2`

Luo funktio jota kutsutaan kun Ohjaimen ko nappi vapautetaan. 

Nimeä funktio joka suoritetaan kun nappi vapautetaan ja laita se  ns `callback` funktion parametriksi.

```python
# Function to run when the event occurs
def run_on_button_released():
    brain.screen.print("Button released!")

# Register event with a callback function.
controller_1.buttonA.released(run_on_button_released)
```

<advanced>
</advanced>