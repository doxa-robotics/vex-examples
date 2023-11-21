category: sound  
signature: brain.play_note(OCTAVE, NOTE, DURATION)  
description: Plays the selected musical note  

# Play Note

Plays the selected musical note.

```python
brain.play_note(OCTAVE, NOTE, DURATION)
```

## How To Use

Choose an octave to replace the **OCTAVE** parameter. The lowest is 1 and the highest is 7.

Choose a note to replace the **NOTE** parameter:

- 0 (C)
- 1 (D)
- 2 (E)
- 3 (F)
- 4 (G)
- 5 (A)
- 6 (B)

Choose a duration for the note to play in milliseconds. You can use of the established options below for the **DURATION** parameter:

- 1000 (whole note plays for 1 second)
- 500 (half note plays for 0.5 seconds)
- 250 (quarter note plays for 0.25 seconds)

Alternatively, you can also use a custom duration in the range of **0 to 1000** milliseconds.

Once a musical note starts playing, the proceeding command will begin executing immediately.

## Example

This example will play a Middle C note for 1 second.

```python
brain.play_note(4, 0, 1000)
```

<advanced>
</advanced>
