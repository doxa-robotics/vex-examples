category: sensing  
signature: vision.largest_object()  
description: Reports information about the largest detected object from a VEX Vision Sensor  

# Largest Object

Reports information about the largest detected object from a VEX Vision Sensor.

```python
vision.largest_object()
```

## How To Use

Configure the Vision Sensor by adding signatures / codes.

A call to the Vision Sensor's `Take Snapshot` command is then required to capture an image in the Vision Sensor prior to using the `Largest Object` command.

The example below will print some information about a detected object onto an IQ Brain's screen.

```python
while True:
    brain.screen.clear_screen()
    brain.screen.set_cursor(1, 1)

    # Take a snapshot with the Vision Sensor with the specified signature and 
    # store the object data into a variable
    vision_object = vision.take_snapshot(signature)

    # Check the variable to see if a valid object was detected when the snapshot
    # was captured. If yes, print the data
    if vision_object is not None:
        brain.screen.print("Center X:", vision.largest_object().centerX)
        brain.screen.next_row()

        brain.screen.print("Center Y:", vision.largest_object().centerY)
        brain.screen.next_row()

        # Take a new snapshot every 0.2 seconds
        wait(0.2, SECONDS)
    else:
        brain.screen.print("No Object Found")
```

The following is a list of properties that can be accessed on the object returned by the `Largest Object` command:

- `id` - A unique ID assigned to each object by the Vision Sensor
- `originX` - The top left X position of the object
- `originY` - The top left Y position of the object
- `centerX` - The center X position of the object
- `centerY` - The center Y position of the object
- `width` - The width of the object
- `height` - The height of the object
- `angle` - The angle of the object
- `exists` - If the Vision Sensor detects the object or not

<advanced>
</advanced>
