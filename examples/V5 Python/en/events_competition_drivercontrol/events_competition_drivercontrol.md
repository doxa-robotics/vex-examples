category: events  
signature: def driver_control():\n\tpass
description: Runs the specified function when a "driver control" mode signal is received from a competition field or competition switch.  

# Competition Driver Control

Runs the specified function when a "driver control" mode signal is received from a competition switch.

```python
def driver_control():
    pass
```

## How To Use

A new competition instance can be created by passing a **driver_control** and **autonomous** callback functions.

Create a **driver_control** function to pass to a competition instance. 

The specified **driver_control** function will run when a "driver control" mode signal is received from a competition switch.

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