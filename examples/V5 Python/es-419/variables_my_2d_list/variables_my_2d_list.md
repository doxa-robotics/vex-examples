category: variables  
signature: my_2d_list = [\n\t[0,0,0],\n\t[0,0,0],\n\t[0,0,0]\n]
description: 2D list variables are used to store multiple lists.

# Variable de Lista 2D

Las variables de lista 2D se utilizan para almacenar listas con varias filas y columnas.

## Cómo Utilizar

Para crear una variable de lista 2D, cree un nombre de variable único y significativo. Esto significa que el nombre de la variable debe describir con precisión la naturaleza de sus valores.

Por ejemplo, una variable de lista 2D llamada "coordenadas" puede usarse para almacenar múltiples conjuntos de valores de coordenadas.

Declare esta lista usando un símbolo igual único '=' después del nombre de su lista seguido de corchetes '[ ]'.

Dentro de estos corchetes, inserte varios conjuntos de corchetes, separados por una coma, así: '[[ ], [ ]]'. Se pueden anidar más de dos conjuntos de corchetes dentro del conjunto de corchetes más externo.

Incluya valores separados por una coma o ',' en sus respectivos corchetes. Si la variable está almacenando cadenas, coloque la coma fuera del encierro '" "'.

Cada conjunto interno de corchetes representa una fila de elementos de lista. El índice del elemento dentro de la fila representa una columna de la lista 2D.

Para acceder al valor de una lista 2D, utilice el nombre de la lista, seguido inmediatamente de dos índices entre corchetes. El primer índice hace referencia a la fila, mientras que el segundo índice hace referencia a la columna de la lista 2D. Tenga en cuenta que los índices de matriz comienzan en 0, no en 1.

Por ejemplo, dada una lista 2D 'coordenadas = [[X1, Y1], [X2, Y2]]', la expresión 'coordenadas[0][0]' devolverá 'X1'. 

## Ejemplo 1

Este ejemplo muestra que a una variable llamada my_list se le asignan dos listas de colores separadas.

```don
my_list = [["Green", "Red", "Blue"], ["Black", "Yellow", "Orange"]]
```

## Ejemplo 2

Este ejemplo muestra que a una variable llamada my_list se le asignan dos listas de números separadas.

```don
my_list = [[1, 2, 3], [4, 5, 6]]
```
<advanced>
</advanced>
