## Ejercicio 1: 

Crear un arreglo de 6 bytes no signados con los siguientes valores iniciales:
{12, 15, 94, 20, 15, 45}.

Crear un arreglo de 6 enteros no signados (2 bytes c/u). Los valores iniciales deben ser: {1200, 1235, 44694, 11920, 50915, 45}.

## Ejercicio 2:

Escribir una rutina que encuentre el mayor de los elementos del array del ejericio anterior formado por elementos de 1 byte. Indicar los cambios que se deberían hacerse en el código para que la rutina escrita se pueda utilizar para encontrar el elemento mayor del arreglo de 2 bytes cada uno (Se deberían hacer menos de 5 modificaciones en el código).

## Ejercicio 3:

Crear un arreglo bidimensional de 4 x 3 celdas, las mismas contienen números no signados de 16 bits (sólo definirlo, colocar valores en el mismo no es necesario).

Escribir la subrutina get_cell que retorne el valor cualquiera de una celda de la matriz de  4 x 3. La subrutina deberá devolver el valor en el registro D, recibirá por stack la dirección de comienzo de la matriz, el número de fila y columna. La primera fila/columna del arreglo se indica con el número cero, mientras que la última con el 3/2. La función deberá invocar a la subrutina chk­_status que verificará que los valores de fila y columna sean válidos. La forma de recepción y envío de parámetros a chk_status la definirá cada grupo según crea más conveniente. Se exige documentación clara al respecto. La función get_cell devuelve el flag de carry en uno si ocurrió un error y en cero si se pudo obtener el valor deseado.
Trabajar con constantes simbólicas en el desarrollo de las funciones.

## Ejercicio 4:

Teniendo en cuenta el ejercicio 3 se pide escribir la función put_cell. La función de la misma es colocar un elemento de 16 bits en la matriz. Queda a criterio  del alumno seleccionar el método de entrega y devolución de parámetros de la función. Se pide correcta documentación al respecto. La función debe contemplar un código de error llegado el caso de que no se pueda colocar el elemento en la matriz (esto ocurre si las filas o columnas son incorrectas). Trabajar con constates simbólicas en el desarrollo de las funciones.


## Ejercicio 5:
		
Crear la estructura biblioteca la misma esta compuesta por 20 estructuras libro. La estructura libro se define de la siguiente manera:

- Autor del libro [max 20 caracteres terminado en cero]
- Nº de inventario [1 byte]
- Tema  [5 bytes]

Cada uno de estos campos será completado con caracteres ASCII.

## Ejercicio 6:

Escribir la subrutina get_author. La misma recibe el número de inventario de un libro y devuelve un puntero al autor del libro y la cantidad de caracteres que contiene el nombre. Se pide que la función reciba por el registro A el número de inventario, devuelva por IX el puntero y por el registro A la cantidad de caracteres del autor. Si el número de inventario no coincide con uno existente en la biblioteca se debe encender el flag de carry.
Se pide modularidad y claridad en la documentación.

## Ejercicio 7:

Se pide escribir la subrutina put_theme. La misma copia el contenido de un arreglo auxiliar en el campo tema de un libro en particular. La subrutina recibe un puntero al arreglo auxiliar y un número de inventario. Queda a criterio del programador elegir la forma en que se reciben los parámetros. El carry debe contemplar algún código de error. Se pide modularidad y documentación completa.


## Ejercicio 8:

Se pide escribir una función que cree un arreglo de punteros con las direcciones de comienzo de los autores de la estructura del ejercicio 6. Queda a criterio del programador el diseño de la función. Se evaluará la modularidad y la correcta documentación.