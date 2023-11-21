category: motion  
signature: MOTOR393.setReversed(true);  
device_class: motor29
description: Reverses the spin direction of a Motor 393 connected to a Motor Controller 29.

# Motor393.setReversed();

Reverses the spin direction of a Motor 393 connected to a Motor Controller 29.

```cpp
Motor393.setReversed();
```

## How To Use

This command reverses the spin direction of a Motor 393.

`Motor393.setReversed();` accepts a Boolean argument of `true` or `false`.

Setting the `Motor393.setReversed(true);` will set the spin directions `forward` and `reverse` to the opposing spin directions. Any following `Motor393.spin();` commands will spin in the direction set by the `Motor393.setReversed();` command.

```cpp
Motor393.setReversed(true);
Motor393.spin(forward);
```

<advanced>
</advanced>