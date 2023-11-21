category: sensing  
signature: Brain.Battery.current()
description: Reports the current of the V5 Brain's battery.

# Akun virrankulutus

ANtaa V5 aivojen akun virrankulutuksen.

```cpp
Brain.Battery.current()
```

## Miten käytetään


`Brain.Battery.current()` antaa desimaaliluvun (muotoa *double*) V5 aivojen akun virrankulutuksen arvona.

Oletusyksikkö on ampeeri (`amp`) välillä **0.0 - 20.0 amps**.

```cpp
Brain.Screen.print("%f", Brain.Battery.current());
```
<advanced>
</advanced>