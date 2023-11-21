category: sensing  
signature: distance.object_size()  
device_class: distance  
description: Reports an estimation of the detected object's size  

# Distance Object Size

Reports an estimation of the detected object's size.

```python
distance.object_size()
```

## How To Use

`Distance Object Size` can be used to approximately determine if a detected object is of a certain size.

There are three defined sizes that can be used for comparison:

- ObjectSizeType.SMALL
- ObjectSizeType.MEDIUM
- ObjectSizeType.LARGE

## Example

The example below prints "Large!" to a VEX IQ Brain's screen if a large object is detected by an IQ Distance Sensor (2nd generation).

```python
if distance.object_size() == ObjectSizeType.LARGE:
    brain.screen.print("Large!")
```

<advanced>
</advanced>





