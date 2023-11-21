category: magnet  
signature: MAGNET.pickup();  
device_class: electromagnet  
description: Energize a Electromagnet to pick up a magnetic object  

# Magnet Pickup

Energize a Electromagnet to pick up a magnetic object.

```cpp
Magnet.pickup();
```

## How To Use

The `Magnet.pickup()` command will energize the Electromagnet to pick up a magnetic object underneath the magnet.

```cpp
Magnet.pickup();
Drivetrain.driveFor(forward, 200, mm);
Magnet.drop();
```

<advanced>
</advanced>






