category: sound  
signature: brain.play_sound(SOUND)  
description: Plays the specified sound effect   

# Play Sound

Plays the specified sound effect.

```python
brain.play_sound(SOUND)
```

## How To Use

Replace the **SOUND** parameter with one of the following sounds to play:
- `SoundType.SIREN`
- `SoundType.WRONG_WAY`
- `SoundType.WRONG_WAY_SLOW`
- `SoundType.FILLUP`
- `SoundType.HEADLIGHTS_ON`
- `SoundType.HEADLIGHTS_OFF`
- `SoundType.TOLLBOOTH`
- `SoundType.ALARM`
- `SoundType.TADA`
- `SoundType.DOOR_CLOSE`
- `SoundType.RATCHET`
- `SoundType.WRENCH`
- `SoundType.SIREN2`
- `SoundType.RATCHET2`
- `SoundType.ALARM2`
- `SoundType.POWER_DOWN`

## Example

The example below plays the siren sound.

```python
brain.play_sound(SoundType.SIREN)
```

Once a sound effect starts playing, the proceeding command will begin executing immediately.

<advanced>
</advanced>
