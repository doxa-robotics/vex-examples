category: variables  
signature: variables_arrays
description: Declares the type, name, length of an array. 

# Array Variables

Declares the type, name, and length of an array. 

```cpp
int myArray[3] = { 1, 2, 3 };
```

## How To Use

Declare what type of data will be stored in your array. 

- `int`
- `double`
- `bool`

Name the array something descriptive and unique. Set the length of the array inside a pair of square brackets `[]` just after the array name. 

```cpp
int turnAngles[3];
```

The values in the array can be declared when creating the array using curly brackets.

```cpp
bool boolArray[2] = { false, true };
```

The values can also be declared individually by index. The index always starts at zero. 

```cpp
// Declare a new array of length 3
double doubleArray[3];

// Assign values to the array by index
doubleArray[0] = 1.5;
doubleArray[1] = 3.14;
doubleArray[2] = 2.18;
```

To read values from an array, provide the index of a specific element in the square brackets.

```cpp
// Read the value at index 2 in integerArray

int value = integerArray[2];
```

## Example

This example will set the array to initial values and then report item #3 (index number 2) from the list to spin a Motor. 

```cpp
int degreesArray[3] = { 30, 60, 90 };
Motor.spinFor(forward, degreesArray[2], degrees);
```

<advanced>
</advanced>