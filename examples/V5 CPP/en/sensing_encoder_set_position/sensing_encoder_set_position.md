category: sensing  
signature: ENCODER.setPosition(position, units);  
device_class: encoder  
description: Sets the Shaft Encoder's position to the given value.

# Encoder Set Position

Sets the Shaft Encoder's position to the given value.

```cpp
Encoder.setPosition(position, units);
```

## How To Use

`Encoder.setPosition()` can be used to set the Shaft Encoder's position to any given positional value.

Usually, `Encoder.setPosition()` is used to set the position 0 to reset the Shaft Encoder's position.

The **units** parameter can be set to **degrees** or **turns**.

```cpp
EncoderA.setPosition(0, degrees);
EncoderB.setPosition(0, turns);
```

<advanced>
</advanced>