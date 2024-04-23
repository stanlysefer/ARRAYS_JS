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
let miArray2 = new Array(3);
miArray[0]= 1;
miArray[1]= 2;
miArray[2]= 3;
consle.log(miArray3);
```
4. declarando un array con elementos de diferentes tipos de datos
```Javascript
let miArray = [1, "dos", true, {nombre: "juan", edad:30}];
consle.log(miArray4);
```