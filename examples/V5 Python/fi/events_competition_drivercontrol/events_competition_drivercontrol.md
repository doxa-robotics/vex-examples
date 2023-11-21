category: events  
signature: def driver_control():\n\tpass
description: Runs the specified function when a "driver control" mode signal is received from a competition field or competition switch.  

# Kilpailu ohjainkäynnistys

Suorittaa halutun funktion kun "ohjainajo" moodi signaali on kilpailuajon alussa saatu.

```python
def driver_control():
    pass
```

## Miten käytetään

Uusi kilpailu esiintymä voidaan luoda kun  **ohjainajo** ja **automaatti** callback funktiot on saatu.

Luo **ohjainkäynnistys** funktio, joka toimii kilpailutilanteessa. 

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