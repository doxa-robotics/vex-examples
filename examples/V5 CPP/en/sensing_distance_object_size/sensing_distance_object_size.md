category: sensing  
signature: DISTANCE.objectSize()  
device_class: distance  
description: Reports an estimation of the detected object's size  

# Distance Object Size

Reports an estimation of the detected object's size.

```cpp
Distance.objectSize()
```

## How To Use

`Distance.objectSize()` can be used to determine if a detected object is of a certain size.

There are three defined sizes that can be used for comparison:
* sizeType::large
* sizeType::medium
* sizeType::small

```cpp
if (Distance.objectSize() == sizeType::large) {
  Brain.Screen.print("Large object detected!");
}
```

<advanced>
</advanced>





