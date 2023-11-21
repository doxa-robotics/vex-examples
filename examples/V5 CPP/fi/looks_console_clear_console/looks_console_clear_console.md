category: looks  
signature: printf("\033[2J\n");  
description: Clears the Print Console and resets the cursor.  

# Console Clear

Clears the Print Console and resets the cursor.

```cpp
printf("\033[2J\n");
```

## How To Use

Using the `printf` command with the special `\033[2J` escape sequence and code will clear the Print Console.

The newline character, `\n` is needed in a `printf` command to output the contents of the Print Console buffer into the Print Console. In this instance, the Print Console will be immediately updated/cleared when this command is executed.

## Example

The example below will print `VEXcode` to the Print Console, wait 2 seconds, and then clear the Console.

```cpp
printf("VEXcode\n");
wait(2, seconds);
printf("\033[2J\n");
```

<advanced>
</advanced>