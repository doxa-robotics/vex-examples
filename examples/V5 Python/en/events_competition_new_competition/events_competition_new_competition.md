category: events  
signature: competition = Competition(driver_control, autonomous)
description: Create a new competition instance  

# New Competition

Create a new competition instance.

```python
competition = Competition(driver_control, autonomous)
```

## How To Use

A new competition instance can be created by passing a **driver_control** and **autonomous** callback functions.

When a **driver control** signal is received from a competition switch, the **driver_control** callback function will be executed.

Similarly, when an **autonomous** signal is received from a competition switch, the **autonomous** callback function will be executed.

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