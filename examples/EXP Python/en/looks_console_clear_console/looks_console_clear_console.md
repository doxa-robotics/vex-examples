category: looks  
signature: print("\033[2J")  
description: Clears the Print Console.  

# Console Clear

Clears the Print Console.

```python
print("\033[2J")
```

## How To Use

The `print` command used with the `\033[2J` command sequence will clear the Print Console.

## Example

The example below will print "VEXcode" and then clear the Print Console after 3 seconds.

```python
print("\033[31mVEXcode")
wait(3, SECONDS)
print("\033[2J")
```

<advanced>
</advanced>
