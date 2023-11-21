category: sound 
signature: Brain.playNote(octave, note, duration);  
device_class: sound  
description: Plays the selected musical note.

# Play Note

Plays the selected musical note.

```cpp
Brain.playNote(octave, note, duration);
```

## How To Use

Choose an octave. The lowest is 1 and the highest is 7. 

Choose a note to play within that octave:
- `C = 0`
- `D = 1`
- `E = 2`
- `F = 3`
- `G = 4`
- `A = 5`
- `B = 6`

Choose a duration for the note to play in **milliseconds**:

- A whole note plays for 1 second (1000 milliseconds)
- A half note plays for 0.5 seconds (500 milliseconds)
- A quarter note plays for 0.25 seconds (250 milliseconds)

Once a musical note starts playing, the proceeding command will begin executing immediately.

## Example

This example will play a Middle C note for 1 second.

```cpp
Brain.playNote(4, 0, 1000);
```

<advanced>
</advanced>