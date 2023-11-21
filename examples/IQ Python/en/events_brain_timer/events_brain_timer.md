category: events  
signature: brain.timer.event(callback, time)  
description: Runs the specified function when the IQ Brain's timer is greater than the specified time value  

# Timer Event

Runs the specified callback function when the IQ Brain's timer is greater than the specified time value.

```python
brain.timer.event(callback, time)
```

## How To Use

The IQ Brain's timer begins at the start of each program.

The `Timer Event` function takes 2 parameters.

The first is the **callback function** parameter. A function will need to be created to pass to the `Timer Event` function.

The second parameter is the time at which the function will run. The **callback function** will run once the IQ Brain's timer is greater than the passed value. The amount of **time** should be in **milliseconds**.

```python
# Call the callback function after 1000 milliseconds
brain.timer.event(callback, 1000)
```

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs.

In the snippet below, "Callback Function Called" will be printed to the VEX IQ's Brain Screen after 10 seconds.

```python
def callback_function():
    brain.screen.print("Timer Elapsed")

brain.timer.event(callback_function, 10000)
```

<advanced>
</advanced>