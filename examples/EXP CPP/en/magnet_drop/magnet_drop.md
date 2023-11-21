category: magnet  
signature: MAGNET.drop();  
device_class: electromagnet  
description: Energize a Electromagnet to drop an attached object  

# Magnet Drop

Energize a Electromagnet to drop an attached magnetic object.

```cpp
Magnet.drop();
```

## How To Use

The `Magnet.drop()` command will release the object that the Electromagnet is currently attached to.

```cpp
Magnet.pickup();
Drivetrain.driveFor(forward, 200, mm);
Magnet.drop();
```

<advanced>
</advanced>





