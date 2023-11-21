category: events  
signature: bumper.pressed(callback)  
device_class: bumper  
description: Runs the specified function when the bumper is pressed.  

# Painokytkintä painettu

Suorittaa halutun funktion kun painokytkintä painettu.

```python
bumper.pressed(callback)
```

## Miten käytetään

Luo funktio, jota kutsutaan, kun painokytkintä on painettu. 

Anna funktiolle nimi ja toiminnot. Nimi välitetään callback - parametrina kun painokytkintä on painettu.

```python
# Function to run when the event occurs
def run_on_bumper_pressed():
    brain.screen.print("Bumper pressed!")
 
# Register event with a callback function
bumper_a.pressed(run_on_bumper_pressed)
```

<advanced>
</advanced>