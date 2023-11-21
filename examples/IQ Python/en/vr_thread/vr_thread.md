category: functions  
signature: vr_thread(function_name)  
description: The VR Thread function must be used to call functions at the global scope of the program.  

# VR Thread

The VR Thread function must be used to call functions at the global level of the program. It can be used to start threads to run simultaneously.

```python
vr_thread(function_name)
```
Notice that the function name is passed as a reference to the `vr_thread()` call rather than calling the function inside a VR Thread such as `vr_thread(function_name())`.

## How To Use

You can take any function you have in the program and pass its reference to `vr_thread()` on the global scope. Using VR Threads are necessary in order for multiple functions to run in parallel. 

The functions will, in general, execute in the order that they are passed into `vr_thread()` calls. If a function is waiting for a command to complete, it will pass program execution to another function, and resume its execution when the other function finishes running, or is also waiting for a command to complete.

The functions that causes threads to switch program execution:

```python
drivetrain.drive_for(FORWARD, 200, MM, wait=True)
drivetrain.turn_for(RIGHT, 90, DEGREES, wait=True)
drivetrain.turn_to_heading(90, DEGREES, wait=TRUE)
drivetrain.turn_to_rotation(90, DEGREES, wait=TRUE)
drivetrain.set_heading(0, DEGREES)
drivetrain.set_rotation(0, DEGREES)
wait(1, SECONDS)

Any user-created function
```

## Example 1

We make a single function that is executed in the global scope with `vr_thread()`. The `move_drivetrain()` function will make the robot move 200 mm and then print when it is done.

```python
def move_drivetrain():
    drivetrain.drive_for(FORWARD, 200, MM)
    brain.screen.print("Done moving")
    brain.screen.next_row()

vr_thread(move_drivetrain)
```

## Example 2

Now we added the `lower_fork()` function. This will move the fork down and print a message when the fork is fully lowered.

We make the call `vr_thread(lower_fork)` **after** the `vr_thread(move_drivetrain)` call. However, because `drivetrain.drive_for(FORWARD, 500, MM)` makes the thread wait, it will switch program execution over to the `lower_fork` function, which will start lowering the fork before the drivetrain completes its movements.

```python
def move_drivetrain():
    drivetrain.drive_for(FORWARD, 500, MM)
    brain.screen.print("Done moving")
    brain.screen.next_row()

def lower_fork():
    fork_motor_group.spin_for(FORWARD, 1700, DEGREES)
    brain.screen.print("Fork lowered")
    brain.screen.next_row()

vr_thread(move_drivetrain)
vr_thread(lower_fork)
```

<advanced>
</advanced>