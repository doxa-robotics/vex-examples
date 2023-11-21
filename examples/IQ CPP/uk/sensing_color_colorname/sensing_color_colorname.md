category: sensing  
signature:  Color9.colorname()
device-class: Color Sensor
description: Reports the name of the color detected by the VEX IQ Color Sensor.

# Color Of

Передає назву кольору, знайденого датчиком кольору VEX IQ. 

```cpp
Color.colorname()
```

## Як це працює

`Color.colorname` може передати один із таких кольорів: 
- `red`
- `red_violet`
- `violet`
- `blue_violet`
- `blue`
- `blue_green`
- `green`
- `yellow_green`
- `yellow`
- `yellow_orange`
- `orange`
- `red_orange`

Перша частина команди - назва пристрою.

```cpp
Color4.colorname()
Color5.colorname()
```

<advanced>
</advanced>