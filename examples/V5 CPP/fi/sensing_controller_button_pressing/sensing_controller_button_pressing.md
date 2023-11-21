category: sensing  
signature: Controller.buttonUp.pressing()  
device_class: controller  
description: Reports if a button on the V5 Controller is pressed.

# Ohjaimen napin painallus

Antaa tiedon jos V5 ohjaimen tiettyä nappia on painettu.


```cpp
Controller.Button.pressing()
```

## Miten käytetään

'controller.buttonUp.pressing()' antaa arvon **True** jos ko nappia on painettu.

'controller.buttonUp.pressing()' antaa arvon **False** jos ko nappia ei ole painettu.

Valitse mitä nappia käsittelet:

* `buttonUp`
* `buttonDown`
* `buttonLeft`
* `buttonRight`
* `buttonX`
* `buttonY`
* `buttonA`
* `buttonB`
* `buttonL1`
* `buttonL2`
* `buttonR1`
* `buttonR2`

```cpp
waitUntil(Controller1.ButtonUp.pressing());
```
<advanced>
</advanced>
