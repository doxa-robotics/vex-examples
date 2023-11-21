category: looks  
signature: CONTROLLER.rumble(rumbleShort);  
device_class: controller  
description: Creates a vibrating effect on your V5 Controller.  

# Ohjainvärinä

Laittaa V5 ohjaimen värisemään.

```cpp
Controller.rumble(".-.-");
```

## Miten käytetään

`Controller.rumble();` komento käyttää V5 ohjaimen värinämoottoria.

Voit säätää värinää "." ja "-" merkeillä. Merkki "." luo lyhyen ja merkki "-" pitkän värinän.

Voit käyttää myös esimääriteltyjä optioita:

* `rumbleLong` on sama kuin `"----"`
* `rumbleShort` on sama kuin `"...."` 
* `rumblePulse` on sama kuin `"-.-."`

```cpp
// The following two lines of code will do the same thing
Controller.rumble("....");
Controller.rumble(rumbleShort);
```

<advanced>
</advanced>