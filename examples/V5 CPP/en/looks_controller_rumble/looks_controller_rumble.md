category: looks  
signature: CONTROLLER.rumble(rumbleShort);  
device_class: controller  
description: Creates a vibrating effect on your V5 Controller.  

# Controller Rumble

Creates a vibrating effect on your V5 Controller.

```cpp
Controller.rumble(".-.-");
```

## How To Use

The `Controller.rumble();` command uses the rumble motor in your V5 controller to provide feedback.

You can create any pattern you want using a combination of "." and "-" characters in the string. The "." character will create a short pulse. The "-" character will create a long pulse.

You can also use predefined rumble options:

* `rumbleLong` is the same as `"----"`
* `rumbleShort` is the same as `"...."` 
* `rumblePulse` is the same as `"-.-."`

```cpp
// The following two lines of code will do the same thing
Controller.rumble("....");
Controller.rumble(rumbleShort);
```

<advanced>
</advanced>