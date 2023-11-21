category: sensing  
signature: CONTROLLER.Screen.column()  
device_class: controller  
description: Reports the column number of the V5 Controller screen cursor location.

# Controller.Screen.column()
# Kursorin sarake
 
Antaa ohjaimen näytöltä kursorin sarakenumeron.

```cpp
Controller.Screen.column()
```

## Miten käytetään

`Controller.Screen.column()` antaa kokonaisluvun välillä **1 to 19**.

```cpp
if (Controller1.Screen.column() > 10) {
}
```

---
V5 Ohjainen näytölle ei voi muuttaa fontin kokoa.

**V5 Ohjain Fonttikoko - Sarakkeiden lukumäärä:**

* Standard Font - 19 saraketta (Oletus)

![brain_screen_info_2](v5_controller_rows_columns.jpg)


<advanced>
</advanced>