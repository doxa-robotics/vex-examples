category: sensing  
signature: Vision.largestObject  
description: Reports the largest object that the vision sensor sees.

# Vision Largest Object

Returns the largest object that the Vision Sensor sees.

```cpp
Vision.largestObject
```

## How To Use

A call to `Vision.takeSnapshot` will need to be made before using the `Vision.largestObject` command.

The `Vision.largestObject` command will return an object of type `vision::object`.

```cpp
// Take a snapshot with the COLOR_SIG signature
Vision.takeSnapshot(COLOR_SIG);

Brain.Screen.print("X: %d", Vision.largestObject.centerX);
Brain.Screen.newLine();
Brain.Screen.print("Y: %d", Vision.largestObject.centerY);
Brain.Screen.newLine();
```

The `Vision.largestObject` is of the type `vision::object` which has these properties which can be accessed.

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