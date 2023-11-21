category: events  
signature: competition = Competition(driver_control, autonomous)
description: Create a new competition instance  

# Uusi kilpailu

Luo uusi kilapilu ilmentymä (ohjelma).

```python
competition = Competition(driver_control, autonomous)
```

## Miten käytetään

uusi kilpailu ilmentymä ottamalla ohjelmaan mukaan **driver_control** ja **autonomous** callback -funktiot.

Kun **driver control** signaali kilpailukytkimestä saadaan, niin suoritetaan **driver_control** callback funktio.

Vastaavasti, kun **autonomous** signaali kilpailukytkimestä saadaan, niin suoritetaan **autonomous** callback funktio.

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