category: variables  
signature: variables_boolean
description: Declares the type, name, and value of a Boolean. 

# Boolean Variable

Stores a **true** or **false** value.

`bool myBoolean = true;`

## How To Use

**Boolean variables** store a **true** or **false** value. Declare with the keyword `bool` in front of a unique and descriptive variable name and set it to equal either `true` or `false`. 

`bool goFast = true;`

Booleans can be used inside of control statement conditionals. 

```cpp
if (goFast) {
  Drivetrain.setDriveVelocity(100, percent);
}
```

<advanced>
</advanced>