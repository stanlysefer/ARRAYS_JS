# Arrays

- Un array es una zona de almacenamiento continuo, donde se pueden introducir varios valor, cada uno de ellos ubicado por la posiscion que ocupa en el array.

- Tambien son conocidos como arreglos o vectores, y cuando son de dos dimensiones son llamados matrices.

- Los arrays nos brinda la capacidad de almacenar una colleccio de elementos y acceder a ellos de manera individual.

- Cada elemento se identifica mediante su posicion en el array, denominada **indice**, y estos indices son siempre secuenciales.

- En Javascript son altamente flexible en terminos de los diferentes tipos de datos que podemos almacenar en cada posición del array.

## crear un array 

1. Declarando un array con elementos en linea 
```Javascript
let miArray = [1, 2, 3];
consle.log(miArray);
```
2. Declarando un array con la sintaxis **new Array()**
```Javascript
let miArray2 = new Array(1, 2, 3);
consle.log(miArray2);
```
3. Declarando un arra con un tamaño especifico utilizando la sintaxis **new Array** y asignamos valores despues:

```Javascript
let miArray3 = new Array(3);
miArray[0]= 1;
miArray[1]= 2;
miArray[2]= 3;
consle.log(miArray3);
```
4. declarando un array con elementos de diferentes tipos de datos
```Javascript
let miArray4 = [1, "dos", true, {nombre: "juan", edad:30}];
consle.log(miArray4);
```

## Accediendo a la informacion de un array 

### propiedad length
- devuelve la cantidad de elementos del array 

### Operador [pos]
- permite acceder  para leer o modificar el elemento pos del array 

### Método at(pos)
- Devuelve el elemento de la posición pos. El parametro admite valores negativos, lo que significa que empieza a contar por el final del array.

```Javascript
const letters = ["A", "B", "C"];
console.log(letters.length);
console.log(letters.[2]);
console.log(letters.[5]);
```

## Añadir o eliminar elementos 
- push(ele1, ele2):añade uno o varios elementos al final del array. Devuelve el tamaño dedl array.
```Javascript
let miArray = [1, 2, 3];
miArray.push(4);
console.log(miArray);
```

- pop(): devuelve el ultimo elemento del array y te lo elimina 
```Javascript
let miArray = [1, 2, 3];
miArray.pop();//Elimina el último elemento del array 
console.log(miArray);
```

- unshift(ele1, ele2): añade un o varios elementos al inicio, devolviendo el tamañodel array depuesmde añadidos
```Javascript
let miArray = [1, 2, 3];
miArray.unshift(0);
console.log(miArray);
```

- shift(): devuelve el primer elemento del array y lo elimina
```Javascript
let miArray = [1, 2, 3];
miArray.shift();
console.log(miArray);
```

- concat(ele1, ele2):concatena dos arrays
```Javascript
let miArray = [1, 2, 3];
let miOtroArray = [4, 5];
let nuevoArray = miArray.concat(miOtroArray);
console.log(miArray);
console.log(miOtroArray);
console.log(nuevoArray);
```

- split(separador): a partir de una cadena, crear un array dividiendo dicha cadena en elementos delimitados por separador
```Javascript
let miString = "Hola, ¿cómo estás?";
let miArray =miString.split(" ");
console.log(miArray);
```

- join(separador): a partir de un array, crea una cadena separadora cada elemento con el separador .

```Javascript
let miArray= ["Hola,", "¿cómo", "estás?"];
let mistring =miArray.join(" ");
console.log(miString);
```

## Búsqueda de elementos den un array 
- includes (elemento): devuelve true o false si el elemento existe o no dentro del array.
- indexOf(elemento): devuelve la prmera aparicion del elemento. Si no existe, devuelve -1.

## Modificar el array o crear fragmentos 
- sloce(inicio, fin): devuelve un array con los elementos desde la posición inicio hasta la posición fin, ambos excluidos.

## Ordenar elementos de un array 
- reverse(): invierte el orden de los elementos del array
- sort(): ordenar el array alfabeticamente
- sort(criterio):ordena el array con el criterio determinado por la funcion criterio .

## Borrar elementos de un ARRAY
- Se puede borrar el contenido de un elemento un array poniedo su valor a null o asignado una cadena vacia " ".
- Para eliminar completamente un elemento del array se utiliza el operador delete.

## recorrido de un array
1. recorree con un bucle clasico, pasando por todos los elementos 

2. recorrer con un while, pasando por todos los elementos.

3. usando la sentencia for..in.

## Arrays multidimensionales
```Javascript
const matrix =[
    [1,2,3],
    [4,5,6],
    [7,8,9]
];
```
- Recorrer una matrix utiliazando bucles anidados


# Ejercicios 

1. dada una lista de números separados por coma, calcular la suma, la mayor, el menor y la media de todos.

2. Introduccior dos cadenas con elementos separados por coma  y con un boton cancatenar las dos cadenas y mostrarlas en pantalla.

3. introducir uno a uno los elementos en un array a través de un boton. Conotro boton se va eliminando el ultimo elemento. siempre que se pulse alguno de los botones se debe mostrar el contenido del array.

4. Introducir un conjunto de números separados por comas. Cuando se  pulsa el boton  "pares" cargar una tabla con los numeros introducidos y luego crear otra que solo in cluya los números pares y mostrarla.