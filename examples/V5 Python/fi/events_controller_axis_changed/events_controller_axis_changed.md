category: events  
signature: controller.axis.changed(callback)  
device_class: controller  
description: Runs the specified function when the controller axis value changes.  

# Ohjaimen tatin asentoa muutettu

Suorittaa määrätyn funktion, kun ohjaimen tatin asentoa muutettu.

```python
controller.axis.changed(callback)
```

## Miten käytetään

Valitse ohjaimen tatti, jota käsitellään.

* `axis1`
* `axis2`
* `axis3`
* `axis4`

Luo funktio ohjaimen tatille , joka käsittelee tatin käyttöä. 

Anna funktiolle nimi, jota käytetään `callback` parametrissa, kun tatin asentoa on muutettu kutsuttaessa itse funktiota.

```python
# Function to run when the event occurs
def run_on_axis_changed():
    brain.screen.print("Axis changed!")

  
# Register event with a callback function.
controller_1.axis1.changed(run_on_axis_changed)
```

<advanced>
</advanced>