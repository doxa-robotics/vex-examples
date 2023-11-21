category: magnet  
signature: MAGNET.drop();  
device_class: electromagnet  
description: Energize a V5 Electromagnet to drop an attached object  

# Magnet Drop

Energize a V5 Electromagnet to drop an attached magnetic object.

```cpp
Magnet.drop();
```

## How To Use

The `Magnet.drop()` command will release the object that the V5 Electromagnet is currently attached to.

```cpp
Magnet.pickup();
Drivetrain.driveFor(forward, 200, mm);
Magnet.drop();
```

<advanced>
</advanced>





