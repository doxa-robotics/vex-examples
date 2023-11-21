category: sensing  
signature: sensing_vision_objects
device_class: vision  
description: Reports the objects the Vision Sensor detects. 

# Vision Objects

Reports all of the objects that the Vision Sensor sees.

```cpp
Vision.objects
```

## How To Use

A call to `Vision.takeSnapshot()` will need to be made before accessing the `Vision.objects` array.

The `Vision.objects` is an array that contains all of the objects that the Vision Sensor detects.


```cpp
Vision.takeSnapshot(COLOR_SIG);
vision::object firstObject = Vision.objects[0];
```
This can be used like any other array. You can access the objects in it with the index of each element.

```cpp
vision::object visionObject = Vision.objects[0];
```

You can also use it in control structures like **for loops**. The `Vision.objectCount` can be used as a loop condition.

The snippet below prints the `centerX` and `centerY` values of each detected object to the VEX V5 Brain.

```cpp
Vision.takeSnapshot(COLOR_SIG);
for(int i = 0; i < Vision.objectCount; i++) {
  Brain.Screen.print("X: %d", Vision.objects[i].centerX);
  Brain.Screen.newLine();
  Brain.Screen.print("Y: %d", Vision.objects[i].centerY);
  Brain.Screen.newLine();
}
```

The objects in the `Vision.objects` are of the type `vision::object` which has these accessible properties.

- `id` - A unique ID assigned to each object by the Vision Sensor, is an `int`
- `originX` - The top left X position of the object, is an `int`
- `originY` - The top left Y position of the object, is an `int`
- `centerX` - The center X position of the object, is an `int`
- `centerY` - The center Y position of the object, is an `int`
- `width` - The width of the object, is an `int`
- `height` - The height of the object, is an `int`
- `angle` - The angle of the object, is a `double`
- `exists` - If the vision sensor detects the object or not, is a `bool`


<advanced>
</advanced>