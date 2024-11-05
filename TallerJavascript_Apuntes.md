Lenguaje MarDown:
Objetivo: Proporcionar una herramienta para documentar codigo
p aspectos tecnicos para compartirlos o tenerlos de referencia 
en si en mi git u otra plataforma.

Markdown es un lenguaje de marcado ligero creado en 2004 poor 
john gruber

el objetivo de su creador fue hacer que la gente pudiera escribir usando un fromato de texto 
plano facil de leer, facil de escribir y con la posibilidad de convertir su documento en html valido

conocer sintaxis MarcDown
1.- Parrafos [Parrafo 1...]

la gran simpleza 


_cursiva_

**negritas**

**_cursiva y negrita_**

~tachado~

**_~cursiva, negrita y tachado~_**

# encabezadonivel 1
## encabezadonivel 2
### encabezadonivel 3
#### encabezadonivel 4
##### encabezadonivel 5
###### encabezadonivel 6

Divisiones

Un bloque de contenido
---
este es otro bloque de contenido

Listas: Podemos utilizar las listas ordenadas y listas desordenadas 

1.-htnl5
2.-css
3.-javascript
4.-ajax
5.-json

-htnl5
-css
-javascript
-ajax
-json


citas podemos dar formato de cita a un texto, anteponiendo a la linea de texto un caracter de mayor que (>).

>la IA en el futuro remplazara muchos profesionales de TI .

> ChatGPT debe potenciar mi aprendizaje, no suprimir mi estado autodidacta
>
>Jhonatanpm


Enlaces

[YouTube](https://www.youtube.com)
[enlace a google](https//www.google.com)

imagenes

![texto alternativo](URLdelaimagen)

tablas


| columna 1 | Columna 2 | Columna 3 |
| --------- | --------- | --------- |
|A          |B          |C          |
|D          |E          |E          |
|           |           |           |


Codigo
Podemos dar formato de codigo a un texto para ello se usa el acento grave (`)

esto es un `codigo` en linea

en _javascript_ una variable se define asi: 

`let saludo = "hola mundo";

pero si queeremos sacar un bloque completo de codigo utilizamos`;


```
let estudiante= "Juan Perez";
let  edad=19;
let is estudiante = true;
```

//**Asi se usan los comentarios de JavaScript de una sola linea**

console.log("Bienvenido al mundo de la programación FrontEnd con JavaScript");

console.log("Esta es otra linea" + "Y se conectan con el simbolo +");

/*_Este es un comentario de mas de una  linea_

En javaScript no eXiste un compilador dado que es un lenguaje
interpretado. Es por ello que tenemos que utilizar la instrucción
console.log("") para poder monitoriar el avance y flujo de
la logica que implementamos. Sin embargo Chrome ofrece unas herramientas para 
los errores
*/

//**_Ahora vamos a trabajar con declaraciones de variables_**
---
```
let estudiante="Juan Pérez";
let edad="19 años";
let isEstudiante="true";
let calificacion=92.3;

console.log("Estudiante: "+estudiante);
console.log("Edad: "+edad);
console.log("Estudia: "+isEstudiante);
console.log(typeof calificacion);
console.log(`El promedio global del estudiante es ${calificacion}`);
```


JavaScript es un lenguaje debilmente tipeado, esto significa que
no es estricto en declararación de tipos de datos. Es decir que no 
fuerza a que inicialmente digas el tipo de dato de la variable. Y
esta puede cambiar en el transcurso de lógica por otro tipo de
datos segun sea la necesidad

```
let num1=50;
let num2=25;
let suma=num1 + num2
let resta=num1-num2;
let mult=num1*num2;
let divicion=num1/num2;


console.log("Suma= "+suma);
console.log("Resta= "+resta);
console.log("Multiplicación= "+mult);
console.log("Divición= "+divicion);

let val1;
let val2;
    val1=prompt("Ingresa el primer numero");
    val2=prompt("Ingresa el segundo numero");

    num1=parseInt(val1);
    num2=parseInt(val2);

    console.log("La suma es "+ (num1 + num2))
```


//**Estructuras de control**
(if, if else, switch)
Estas estructuras permiten ejecutar bloques de codigo
segun el resultado de una conducta

```
let EdadA=17;

//_Estructura de control usando if_
if(EdadA >= 18){
    console.log("Eres un adulto y debes registrarte en el SAT")
}
```
---
//**Estructura de control usando if/else**
```
if(EdadA >= 18){
    console.log("Eres un adulto y debes registrarte en el SAT")
}else{
    console.log("Todabia no pagaras impuestos")
}
```
---
//1.- **_Operadores aridmeticos_**
```
let a=10;
let b=5;
console.log(a + b); //suma
console.log(a - b); //resta
console.log(a * b); //multiplicacion
console.log(a / b); //division
console.log(a % b); //modulo
```
---
//_operadores de asignacion_
```
let X=10;
X += 5; //X=15
X -= 2; //X=13
X *= 3; //X=39
X /= 3; //X=13
X %= 15; //X=3
```
---
//_operadores de comparacion_
```
let A=5; let B=`5`;
console.log(A == B); //compara solo el valor
console.log(A === B); //compara el valor y el tipo
console.log(A != B);
console.log(A !== B);
console.log(A > 3);
console.log(A <= 5);
```
---
// _estructuras de control if/false anidado_
```
let cargo = 200

if (cargo >= 100 && cargo <= 150) {
alert("Impuesto bajo")
} else if (cargo >= 151 && cargo <= 200) {
alert("impuesto medio")
} else {
    alert("revisar el tabulador")
}


alert("Estamos en el archivo EstructuraCiclo.js")

// Estructuras de control for
for( let i = 0;i <= 10; i++) {
    console.log ("No iteracion:" + i)
}

let contador = 1

while (contador < 10 ) {
    console.log(" [while ]No iteracion" + contador)
    contador++
}
```

//~estructura de control do/while~
```
let numero=1

do {
    console.log(" [do/while] no iteracion" + numero)
    numero++
} while (numero < 10)
```
// ~for in~ 
// este bucle itera sobre las propiedades enumerables de un objeto.
```
let estudiante = { nombre: "Juan Perez", edad:18, calificacion:70}
for (let propiedad in estudiante) {
console.log(propiedad + ":" + estudiante[propiedad]
)
}
```
//_for... of_
// este ciclo itera sobre los valores de un objeto iterable (como un array).
```
let mis_numeros = [10, 20, 30, 40, 50]

for (let numero of mis_numeros) {
    console.log(numero)
}
```
