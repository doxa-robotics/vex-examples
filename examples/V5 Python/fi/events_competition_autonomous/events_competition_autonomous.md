category: events  
signature: def autonomous():\n\tpass
description: Runs the specified function when a "autonomous" mode signal is received from a competition field or competition switch.  

# Kilpailu automaattikäynnistys

Suorittaa halutun funktion kun "automaatti" moodi signaali on kilpailuajon alussa saatu.

```python
def autonomous():
    pass
```

## Miten käytetään

Uusi kilpailu esiintymä voidaan luoda kun  **driver_control** ja **automaatti** callback functiot on saatu.

Luo **automaatti** funktio, joka toimii kilpailutilanteessa. 

Tämä **automaatti** funktio suoritetaan kun "automaatti" moodi signaali on kilpailussa saatu.

```python
# Function to run when the "driver control" signal is received
def driver_control():
    brain.screen.print("driver control signal received")

# Function to run when the "autonomous" signal is received
def autonomous():
    brain.screen.print("autonomous signal received")

# Create a new Competition instance
competition = Competition(driver_control, autonomous)
```


<advanced>
</advanced>