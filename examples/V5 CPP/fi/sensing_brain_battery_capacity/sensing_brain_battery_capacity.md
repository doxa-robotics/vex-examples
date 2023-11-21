category: sensing  
signature: Brain.Battery.capacity()  
description: Reports the capacity of the V5 Brain's battery.

# Akun kapasiteetti

ANtaa V5 akun kapasiteetin.

```cpp
Brain.Battery.capacity()
```

## Miten käytetään


`Brain.Battery.capacity()` antaa kokonaisluvun muotoa **integer** ja se vastaa akun kapasiteettia yksikössä `percent` (%) välillä **0% - 100%**.

```cpp
Brain.Screen.print("%d", Brain.Battery.capacity());
```

<advanced>
</advanced>