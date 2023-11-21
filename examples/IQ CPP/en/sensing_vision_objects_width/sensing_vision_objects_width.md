category: sensing  
signature: VISION.objects[0].width;  
device_class: vision  
description: Reports the width of a detected object from the Vision Sensor.

# Objects width

Reports the width of a detected object from the Vision Sensor.

```cpp
Vision.objects[index].width
```

## How To Use

In order to use `Vision.objects[index]`, use the following steps:

1. Configure your Vision Sensor using the Robot Configuration window.
2. Use `Vision.takeSnapshot()` to capture a Vision Sensor image and look for a signature / color code.
3. Use `Vision.objects[index].exists` to check if the Vision Sensor detected the requested signature / color code. 

Once the Vision Sensor detects an object, you can use other Vision blocks to learn more about the object detected. 

* Use the **index** to grab which detected object you want to learn more information about. The largest object will be in the front, such that `Vision.objects[0]` returns the largest object.
* Use `Vision.objectCount` to determine how many objects were detected of that requested signature / color code.
* Use can get the following information about each objects: `angle`, `centerX`, `centerY`, `height`, `width` and `exists`.

---

`Vision.objects[index].width` reports how wide the object is in pixels. It returns a value of **2 - 316 px**.

```cpp
Brain.Screen.print(MyVision.objects[1].width);
```

<advanced>
</advanced>