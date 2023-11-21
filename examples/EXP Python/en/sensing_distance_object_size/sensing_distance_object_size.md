category: sensing  
signature: distance.object_size()  
description: Reports the size of an object using Distance Sensor.

# Object Size

Reports the size of an object the Distance Sensor detects.  

```
distance.object_size()
```

## How To Use

Determines the size of the object detected (none, small, medium, large) based on the amount of light reflected and returned to the sensor.


If an object is found, the function will return `ObjectSizeType.SMALL`, `ObjectSizeType.MEDIUM`, or `ObjectSizeType.LARGE`.

If there is no object found, the function will return `ObjectSizeType.NONE`.
	
<advanced>
</advanced>
