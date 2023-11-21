category: variables  
signature: my_2d_list = [\n\t[0,0,0],\n\t[0,0,0],\n\t[0,0,0]\n]
description: 2D list variables are used to store multiple lists.

# 2D List Variable

2D list variables are used to store lists with multiple rows and columns.

## How To Use

To create a 2D list variable, create a unique and meaningful variable name. This means that the variable name should accurately describe the nature of its values.

For example, a 2D list variable name `coordinates`  can be used to store multiple sets of coordinate values.

Declare this list using a single equal symbol `=` after your list name followed by square brackets `[ ]`.

Inside these square brackets, insert multiple sets of square brackets, separated by a comma, like so: `[[ ], [ ]]`. More than two sets of square brackets can be nested within the outer-most set of square brackets.

Include values that are separated with a comma or `,` in their respective brackets. If the variable is storing strings, place the comma outside of the enclosing `" "`.

Each inner set of brackets represents a row of list items. The index of the item within the row represents a column of the 2D list.

To access the value of within a 2D list, use the name of the list, immediately followed by two indexes enclosed in square brackets. The first index references the row, while the second index references the column in the 2D list. Keep in mind that array indexes begin at 0, not 1.

For example, given a 2D list `coordinates = [[X1, Y1], [X2, Y2]]`, the expression `coordinates[0][0]` will return `X1`. 

## Example 1

This example shows a variable called my_list being assigned two separate lists of colors.

```don
my_list = [["Green", "Red", "Blue"], ["Black", "Yellow", "Orange"]]
```

## Example 2

This example shows a variable called my_list being assigned two separate lists of numbers.

```don
my_list = [[1, 2, 3], [4, 5, 6]]
```
<advanced>
</advanced>
