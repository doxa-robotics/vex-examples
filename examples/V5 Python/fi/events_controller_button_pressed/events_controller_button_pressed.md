category: events  
signature: controller.button.pressed(callback)  
device_class: controller  
description: Runs the specified function when the controller button is pressed.  

# Ohjaimen nappia painettu

Suorittaa tietyn funktion kun Ohjaimen tiettyä nappia on painettu.

```python
controller.button.pressed(callback)
```

## Miten käytetään

Valitse ohjaimen nappi (kts ohjaimesta merkinnät napeille).

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

YLuo funktio , jota kutsutaan kun ohjaimen ko. nappia on painetttu. 

Anna fuktiolle nimi, joka välitetään callback` paramettrissa, kun funktion toiminta suoritetaan nappia painettaessa.

```python
# Function to run when the event occurs
def run_on_button_pressed():
    brain.screen.print("Button pressed!")

# Register event with a callback function.
controller_1.buttonA.pressed(run_on_button_pressed)
```

<advanced>
</advanced>