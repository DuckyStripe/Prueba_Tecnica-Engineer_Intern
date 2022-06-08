# Prueba_Técnica-Engineer_Intern

_Prueba técnica para obtener puesto de interno_

## Prueba 🚀

_Consiste en 3 problemas, los cuales los puedes realizar en el lenguaje que mas te agrade._

### Ejercicio 1 📋

_Dado un integer, escribe una función que regrese la suma todos sus dígitos. Es decir, para el integer 12345 las suma de sus dígitos es: 1+2+3+4+5 = 15_ 
 
_Definición de la función_
_digitsSum(inputInt: integer): integer_
 
_Casos de ejemplo_
 
_●	Con inputInt = “999”, la salida debería ser digitsSum(inputInt ) = 27;_
_●	Con inputInt = “9184501”, la salida debería ser  digitsSum(inputInt ) = 28;_
_●	Con inputInt = “12345”, la salida debería ser  digitsSum(inputInt ) = 15;_


```
const inputInt = (numero) => {
    //Convertimos la entrada a string
    const cadena = numero.toString();
    //creamos un array
    let array=[];
    //Agregamos cada valor del numero a un array 
    for (let i = 0; i < cadena.length; i++) {
        array.push(cadena[i]);
    }
    let contador=0;
    for (let j = 0; j < cadena.length; j++){
        contador+=parseInt(cadena[j]);
    }
    console.log(contador);
}
```

### Ejercicio 2 🔧

_Palíndromos_
 
_Dado un string, escribe una función para verificar si es un palíndromo. Un palíndromo es un texto que se lee igual de izquierda a derecha que de derecha a izquierda. Las palabras:salas, oso, reconocer y oro son palíndromos._
 
_Definición de la función_ 
 
_+	isPalindrome(inputStr: string): boolean_
 
_Casos de ejemplo_
 
_●	Con inputStr = “aabaa”, la salida debería ser isPalindrome(inputStr) = true;_
_●	Con inputStr = “abac”, la salida debería ser  isPalindrome(inputStr) = false;_
_●	Con inputStr = “salas”, la salida debería ser  isPalindrome(inputStr) = true;_

```
const esPalindromo = (cadena) => {
    //pasamos la cadena a minusculas
    const cadenaRevisar =cadena.toLowerCase();
    let bandera;
    //creamos una cadena invertida para evaluarla despues
    const cadenaInvertida = cadenaRevisar.split("").reverse().join("");
    if (cadenaInvertida === cadenaRevisar){
        bandera=true;
        return console.log(bandera);
    }else{
        bandera=false;
        return console.log(bandera);
    }

}
```
### Ejercicio 3 🖇️

_Producto de elementos adyacentes_
 
_Dado un arreglo de enteros, encuentra el par de elementos adyacentes tales que su producto sea el más grande y devuelve dicho producto._
_Se consideran como elementos adyacentes aquellos que se encuentren a la izquierda o a la derecha, es decir, dado el arreglo [3, 6, -2, 5] los elementos adyacentes serían:_
 
_●	3 y 6 => 3 * 6 = 18_	 
_●	6 y-2 => 6 * -2 = -12_ 
_●	-2 y 5 => 5 * -2 = -10_ 
 
_La función debería devolver 18 dado que es el producto de adyacentes más grande._ 
 
_Definición de la función_
 
_+	maxAdjacentProd(inputArray: array): integer_
 
_Casos de ejemplo_ 
 
_●	Con inputArray= [3 , 6, -2, -5, 7, 3]  la salida debería ser maxAdjacentProd(inputArray) = 21;_ 
 
_●	Con inputArray=[5 , 1, 2, 3, 1, 4]  la salida debería ser  maxAdjacentProd(inputArray) = 6;_ 
 
_●	Con inputArray=[-23 , 4, -3, 8, -12]  la salida debería ser  maxAdjacentProd(inputArray) = -12;_ 


```
const inputArray = (array) => {
    //variable temporal para guardar el valor mas grande 
    let temp=Number.NEGATIVE_INFINITY;   
    //Iteramos en el array 
    for (let i=0; i< array.length-1; i++){
        //Si el valor de la multiplicacion es mayor que el valor guardado
        if(array[i]*array[i+1] > temp){
            //guardamos la salida
            temp=array[i]*array[i+1];  
        }
    }
    console.log(temp);
}
inputArray([-23 , 4, -3, 8, -12]);
```


## Despliegue 📦

_Este proyecto esta fue realizado con JavaScript y corriendo con node JS_

## Construido con 🛠️

* [JavaScript](https://developer.mozilla.org/es/docs/Web/JavaScript) - Lenguaje para la parte lógica
* [NodeJS](https://nodejs.org/es/) - Entorno de ejecución



## Autor ✒️

* **Luis Alejandro Canchola Pedraza** - *Web Developer Jr*

## Redes 📄
* **Github** - [Github](https://github.com/DuckyStripe)
* **Linkedin** - [Linkedin](https://www.linkedin.com/in/luis-alejandro-canchola-pedraza-a542b8173/)


