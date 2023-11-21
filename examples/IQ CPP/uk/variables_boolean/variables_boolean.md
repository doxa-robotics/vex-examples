category: variables  
signature: variables_boolean
description: Declares the type, name, and value of a Boolean. 

# Boolean Variable

Зберігає значення **true** або **false**.

`bool myBoolean = true;`

## Як це працює

**Логічні змінні** зберігають значення **true** або **false**. Оголошується ключовим словом `bool` перед унікальною і характерною назвою змінної, присвоюється значення `true` або `false`. 

`bool goFast = true;`

Логічні змінні можна використати всередині умовних виразів керування. 

```cpp
if (goFast) {
  Drivetrain.setDriveVelocity(100, percent);
}
```

<advanced>
</advanced>