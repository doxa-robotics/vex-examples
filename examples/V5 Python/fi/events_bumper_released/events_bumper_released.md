category: events  
signature: bumper.released(callback)  
device_class: bumper  
description: Runs the specified function when the bumper is released.  

## Painokytkin vapautettu

Suorittaa halutun funktion kun painokytkin vapautetaan

```python
bumper.released(callback)
```


## Miten käytetään

Luo funktio, jota kutsutaan, kun painokytkin on vapautettu. 

Anna funktiolle nimi ja toiminnot. Nimi välitetään callback - parametrina kun painokytkin on vapautettu.

```python
# Function to run when the event occurs
def run_on_bumper_released():
    brain.screen.print("Bumper released!")
 
# Register event with a callback function
bumper_a.released(run_on_bumper_released)
```

<advanced>
</advanced>