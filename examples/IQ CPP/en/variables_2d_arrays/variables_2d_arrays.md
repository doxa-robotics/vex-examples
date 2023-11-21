category: variables  
signature: variables_2d_array
description: Declares the type, name, length of a 2D array. 

# 2D Array Variables

Declares the type, name, length of a 2D array. 

```cpp
int my2DArray[3][3] = { 
  { 0, 1, 2 },
  { 3, 4, 5 },
  { 6, 7, 8 },
};
```

## How To Use

Declare what type of data will be stored in your 2D array. 

- `int`
- `double`
- `bool`

Name the array something descriptive and unique. Set the array dimensions inside 2 pairs of square brackets `[]` just after the array name. 

```cpp
// Declare a new 2D array with 3 rows and 3 columns

int my2DArray[3][3];
```

The values in the array can be assigned when creating the array using curly brackets.

```cpp
int my2DArray[3][3] = { 
  { 0, 1, 2 },
  { 3, 4, 5 },
  { 6, 7, 8 }
};
```

The values can also be declared individually by index. The index always starts at zero. 

```cpp
// Declare a new turnAngles array with 3 rows and 3 columns
int turnAngles[3][3];

// Assign values by index
int turnAngles[0][0] = 45;
int turnAngles[0][1] = 90;
int turnAngles[0][2] = 180;
int turnAngles[1][0] = 270;
```

To read values from an array, provide the index of the specific element in the square brackets.

```cpp
// The angle variable will be assigned the value of 270

int angle = turnAngles[1][0];
```

## Example

This example shows a **double** 2D array called `myAngles` that will be a 2D array of angles.

```cpp
double myAngles[2][3] = {
  {45.5, 90.0, 88.2},
  {25.0, 75.5, 45.0}
};
```

<advanced>
</advanced>