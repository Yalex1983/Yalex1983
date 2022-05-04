# Entrega Tarea 11 JavaScript

## ejercicio_1.js
Escribir un programa que solicite al usuario que ingrese su nombre. El nombre se debe almacenar en una variable llamada nombre. A continuación, se debe mostrar en pantalla el texto “Ahora estas en la matrix, [usuario]”, donde “[usuario]” se reemplazará por el nombre que se haya ingresado.
```javascript
var usuario = prompt("Ingresen su nombre : ");
console.log("Ahora estás en la matrix, " + usuario);
```
## ejercicio_2.js
Escribir un programa que solicite al usuario ingresar un número con decimales y almacenarlo en una variable, el programa debe solicitar al usuario que ingrese un número entero y guardarlo en otra variable. En una tercera variable se deberá guardar el resultado de la suma de los dos números ingresados por el usuario. Por último, se deberá mostrar en pantalla el texto “El resultado de la suma es [suma]”, donde “[suma]” se reemplazará por el resultado de la operación.
```javascript
var decimal = parseFloat(prompt("Ingrese un numero decimal: "));
var entero = parseInt(prompt("Ingrese un numero entero: "));
var suma = decimal + entero
console.log("El primer numero es: " + decimal);
console.log("El segundo numero es: " + entero);
console.log("El resultado de la suma es: " + suma);
```
### ejercicio_3.js
Escribir un programa que solicite al usuario dos números y los almacene en dos variables. En otra variable, almacenará el resultado de la suma de esos dos números y luego mostrará ese resultado en pantalla. A continuación, el programa debe solicitar al usuario que ingrese un tercer número, el cual se debe almacenar en una variable. Por último, mostrara en pantalla el resultado de la multiplicación de este nuevo número por el resultado de la suma anterior.
```javascript
var pri_num = parseFloat(prompt("Ingrese el primer número: "));
var seg_num = parseFloat(prompt("Ingrese el segundo número: "));
var suma =pri_num+seg_num
console.log("El primer numero es: " + pri_num);
console.log("El segundo numero es: " + seg_num);
console.log("El resultado de la suma es: " + suma);
var ter_num =  parseFloat(prompt("Ingrese el tercer número: "));
var mult = suma * ter_num
console.log("El tercer numero es: " + ter_num);
console.log("El resultado de la multiplicación es: " + mult);
```
### ejercicio_4.js
Escribir un programa que solicite al usuario ingresar la cantidad de kilómetros recorridos por una motocicleta y la cantidad de litros de combustible que consumió durante ese recorrido. Mostar el consumo de combustible por kilómetro
```javascript
var kilometros = parseFloat(prompt("Ingrese los kilometros recorridos: "));
var consumo = parseFloat(prompt("Ingrese los litros de combustible consumidos: "));
console.log("los kilometros recorridos son : " + kilometros + " Km");
console.log("El consumo de combustible es : " + consumo + " litros")
var litrosxKm =kilometros/consumo
console.log("El consumo por kilometro es : " + litrosxKm + " litros")
```
### ejercicio_5.js
Escribir un programa que solicite al usuario el ingreso de una temperatura en escala Fahrenheit (debe permitir decimales) y le muestre el equivalente en grados Celsius. La fórmula para este cálculo es Celsius = (5/9) * (Fahrenheit-32)
```javascript
var tem_far = parseFloat(prompt("Ingrese la tempreatura en Fahrenheit: "));
var temp_celsius = parseFloat((5/9) * (tem_far - 32));
console.log("La temperatura en grados Fahrenheit es: " + tem_far);
console.log("la temperatura en grados Celsius es: " + temp_celsius);
```
### ejercicio_6.js
Escribir un programa que solicite al usuario ingresar tres números para luego mostrarle el promedio de los tres.
```javascript
var num_1 = parseFloat(prompt("Ingrese el primer número: "));
var num_2 = parseFloat(prompt("Ingrese el segundo número: "));
var num_3 = parseFloat(prompt("Ingrese el tercer número: "));
var prom = (num_1+num_2+num_3)/3
console.log("El primer número es: " + num_1);
console.log("El segundo número es: " + num_2);
console.log("El tercer número es: " + num_3);
console.log("El promedio de los números es: " + prom);
```
### ejercicio_7.js
Escribir un programa que solicite al usuario un número y le reste 15%, almacenando todo en una única variable. A continuación, mostrar el resultado final en pantalla.
```javascript
var numero = parseFloat(prompt("Ingrese el un número: "));
console.log("El número ingresado es: " + numero);
var por100 = (numero - (numero*0.15))
console.log("descontando el 15% queda : " + por100);
```
### ejercicio_8.js
Escribir un programa que solicite al usuario el ingreso de dos palabras, las cuales se guardarán en dos variables distintas. A continuación, almacenará en una variable la concatenación de la primera palabra, más un espacio, más la segunda palabra. Mostar este resultado en pantalla.
```javascript
var palabra_1 = (prompt("Ingrese la primera palabra: "));
var palabra_2 = (prompt("Ingrese la segunda palabra: "));
console.log("La primera palabra es: " + palabra_1);
console.log("la segunda palabra es: " + palabra_2);
var union = palabra_1+ " " + palabra_2
console.log(union);
```
### ejercicio_9.js
Escribir un programa que solicite al usuario el ingreso de un texto y almacene ese texto en una variable. A continuación, mostraren pantalla la primera letra del texto ingresado. Luego solicitar que ingrese un número menor a la cantidad de caracteres que tiene el texto que ingresó (por ejemplo, si escribe la palabra “HOLA”, tendrá que ser un numero entre 0 y 3) y almacenar ese número en una variable llamada índice. Mostar en pantalla el carácter del texto ubicado en la posición dada por índice.
```javascript
let texto = (prompt("Ingrese un texto: "));
console.log("El texto es: " + texto);
console.log("La primera letra del texto es :" + texto.charAt(0));
let indice = (prompt("Ingrese un numero positivo nenor a " + texto.length));
console.log("El numero menor que " + texto.length + " es: " + indice)
console.log("El caracter en la posición " + indice +" es: " + texto.charAt(indice));
```
### ejercicio_10.js
Escribir un programa que solicite al usuario que ingrese cuántos shows musicales ha visto en el último año y almacene ese número en una variable. A continuación, mostrar un valor de verdad (True o False) que indique si ha visto más de tres shows
```javascript
let show = (prompt("Cuantos Shows musicales a visto en el último año?: "));
console.log(" Shows vistos en el ultimo año: " +show)

if (show <=3){
  console.log(false)   
}
else{
  console.log(true)  
}
```
### ejercicio_11.js
Escribir un programa que le solicite al usuario ingresar una fecha formada por números, donde los primeros dos representan el día, los siguientes dos el mes y los últimos cuatro el año (DDMMAAAA). Finalmente, mostrar al usuario la fecha con formato DD / MM / AAAA.
```javascript
let fecha = (prompt("Ingrese un numeroformato fecha DDMMAAA: "));
console.log(" Fecha en formato DDMMAAAA: " + fecha)
console.log(fecha.charAt(0)+fecha.charAt(1)+"/"+fecha.charAt(2)+fecha.charAt(3)+"/"+fecha.charAt(4)+fecha.charAt(5)+fecha.charAt(6)+fecha.charAt(7))
```
### ejercicio_12.js
Escribir un programa para solicitar al usuario el ingreso de un número entero y que luego imprima un valor de verdad dependiendo de si el número es par o no. Recordar que un número es si el resto, al dividirlo por 2, es 0.
```javascript
let num = (prompt("Ingrese un número entero: "));
console.log(" El número entero es: " + num)

if (num%2==0){
  console.log(true)   
}
else{
  console.log(false)  
} 
```
### ejercicio_13.js
Escribir un programa que solicite al usuario su edad y la guarde en una variable. Que luego solicite la cantidad de artículos comprados en una tienda y la almacene en otra variable. Finalmente, mostrar en pantalla un valor de verdad (True o False) que indique si el usuario es mayor de 18 de edad y además compró más de 1 articulo.
```javascript
let edad = (prompt("Ingresa tu edad: "));
console.log(" Tu edad: " + edad);
let articulo = (prompt("Ingrese la cantidad de artículos comprados: "));
console.log("Artículos comprados: " + articulo)

if (edad>=18 && articulo >=2){
  console.log(true)   
}
else{
  console.log(false)  
}
```
### ejercicio_14.js
Escribir un programa que, dada una cadena de texto por el usuario, imprima True si la cantidad de caracteres en la cadena es un número inpar, o False si no lo es.
```javascript
let texto = (prompt("Ingrese una Frase: "));
console.log("La Frase es: " + texto);

if (texto.length%2 ==0){
  console.log(true)   
}
else{
  console.log(false)  
}
```
### ejercicio_15.js
Escribir un programa que le pida al usuario ingresar dos palabras y las guarde en dos variables, que luego inprima True si la primera palabra es un menor que la segunda o False si no lo es.
```javascript
let palabra1 = (prompt("Ingrese la primera palabra: "));
let palabra2 = (prompt("Ingrese la segunda palabra: "));
if (palabra1.length > palabra2.length){
  console.log ("Una Palabra " + palabra1);
  console.log ("Otra Palabra " + palabra2);
  console.log (true);
}
else{
  console.log ("Una Palabra " + palabra1);
  console.log ("Otra Palabra " + palabra2);
  console.log (false);
}
```
### ejercicio_16.js
Escribir un programa para pedir al usuario su nombre y luego el nombre de otra persona, almacenando cada nombre en una bariable. Luego mostrar en pantalla un valor que indique si: los nombres de ambas personas comienzan con la misma letra ó si terminan con la misma letra. Por ejemplo, silos nombres ingresados son Maria y Marcos, se mostrará True, ya que ambos comienzan con la misma letra. Si los nombres son ricardo y Gonzalo se mostrará True, ya que ambos terminan con la misma letra. Si los nombres son Florencia y Laurato se mostrará False, ya que no coinciden ni la primera ni la última letra.
```javascript
let nombre1 = (prompt("Ingresa tu nombre: "));
let nombre2 = (prompt("Ingrese otro nombre: "));

if (nombre1.charAt(0)==nombre2.charAt(0)|| nombre1.charAt(nombre1.length - 1)== nombre2.charAt(nombre2.length - 1)){
    console.log("Tu nombre: " + nombre1);
    console.log("Otro Nombre: " + nombre2);
    console.log(true);
}
else{
    console.log("Tu nombre: " + nombre1);
    console.log("Otro Nombre: " + nombre2);
    console.log(false);
}
```
### ejercicio_17.js
Escribir un programa que, dado un numero entero, muestre su valor absoluto. Recordar que, para los numeros positivos su valor absoluto es igual al numero (el valor absoluto de 52 es 52), mientras que, para los negativos, su valor absoluto es el número multiplicado por -1 ( el valor absoluto de -52 es 52).
```javascript
let numero = parseFloat(prompt ("Ingrese un Número: "));
let aux

if (numero < 0){
    aux = numero * -1
}
else{
    aux = numero
}
console.log("Numero Ingresado: " + numero);
console.log("Numero: " + aux);
```
### ejercicio_18.js
Escribir un programa que solicite al usuario el ingreso de dos números diferentes y muestre en pantalla al mayor de los dos.
```javascript
let numero_1 = parseFloat(prompt("Ingrese el primer numero: "));
let numero_2 = parseFloat(prompt("Ingrese el segundo numero: "));
let aux
if(numero_1 > numero_2){
    aux = numero_1;
}
else{
    aux = numero_2;
}
console.log("El Primer valor ingresado es: " + numero_1);
console.log("El Segundo numero ingresado es: " + numero_2);
console.log("El numero mayor es: " + aux);
```
### ejercicio_19.js
Escribir un programa que solicite al usuario una letra y, si es vocal, muestre el mensaje “Es vocal”. Verificar si el usuario ingresó un String de mas de un carácter y, en ese caso, informarle que no se puede procesar el dato.
```javascript
let letra = prompt("Ingrese una letra : ");
function esVocal(letra){
  if(letra.length !== 1){
    console.log("No se puede procesar el dato, debe ser solo una letra")
  }
    else if(["a", "e", "i", "o", "u"].includes(letra.toLowerCase())){
    console.log("la letra: " + letra)
    console.log("Es vocal")
    }
    else {
    console.log("la letra: " + letra)
    console.log("No es vocal")
  }
}
esVocal(letra);
```
### ejercicio_20.js
Escribir un programa para solicitar al usuario tres números y mostrar en pantalla el menor de los tres.
```javascript
let num_1 = parseInt(prompt("Ingrese el primer número: "));
let num_2 = parseInt(prompt("Ingrese el segundo número: "));
let num_3 = parseInt(prompt("Ingrese el tercer número: "));

if (num_1<= num_2 && num_1<=num_3){
    menor= num_1;
}
else if (num_2 < num_1 && num_2 <=num_3){
    menor = num_2;
}  
else{
    menor = num_3
}
console.log("El menor de los tres números es: "+ menor)
```


