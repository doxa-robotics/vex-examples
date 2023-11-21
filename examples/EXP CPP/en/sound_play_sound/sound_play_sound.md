category: sound  
signature: Brain.playSound(sound);  
description: Plays the sound effect that is entered into the parentheses.

# Play Sound

Plays the specified sound effect through the EXP Brain's Speakers.

```cpp
Brain.playSound(sound);
```

## How To Use

Replace `sound` with one of the following sounds to play.

- `siren`
- `wrongWay`
- `wrongWaySlow`
- `fillup`
- `headlightsOn`
- `headlightsOff`
- `tollBooth`
- `alarm`
- `tada`
- `doorClose`
- `ratchet`
- `wrench`
- `siren2`
- `ratchet2`
- `alarm2`
- `powerDown`

## Example

The example below plays the **siren** sound.

```cpp
Brain.playSound(siren);   
```

Once a sound effect starts playing, the proceeding command will begin executing immediately.

<advanced>
</advanced>