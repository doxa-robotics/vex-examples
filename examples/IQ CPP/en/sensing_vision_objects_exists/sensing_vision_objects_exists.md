category: sensing  
signature: VISION.objects[0].exists;  
device_class: vision  
description: Reports if the Vision Sensor detects a configured object. 

# Objects exists

Reports if the Vision Sensor detects a configured object. 

An object will need to be configured before the `Vision.objects[index].exists` command can detect it.

```cpp
Vision.objects[index].exists
```

## How To Use

Make sure you specify the Vision Sensor when using this command. 


`Vision.objects[index].exists` reports **true** when the Vision Sensor detects a configured object.

`Vision.objects[index].exists` reports **false** when the Vision Sensor does not detect a configured object.

Before the `Vision.objects[index].exists` can report reports a **true** or **false** value, `Vision.takeSnapshot()` will need to be used.


```cpp
if(Vision.objects[0].exists){

}
```

<advanced>
</advanced>