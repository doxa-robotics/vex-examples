category: motion  
signature: MOTOR393.stop();  
device_class: motor29
description: Stops a Motor393 connected to a Motor Controller 29.

# Motor393 Stop

Stops a Motor393 connected to a Motor Controller 29.

```cpp
Motor393.stop();
```

## How To Use

This command stops a Motor393 from spinning.

## Example

This example will spin the Motor393 for three seconds and then stop.

```cpp
Motor393.spin(forward);
wait(3, seconds);
Motor393.stop();
```

<advanced>
</advanced>