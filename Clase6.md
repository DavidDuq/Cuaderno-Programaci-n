## CLASE 6 : **INTRODUCCIÓN A C**      
____
**FECHA** : 18 DE NOVIEMBRE DEL 2022
___
### INTRODUCCIÓN GENERAL 
>Dennis Ritchie es  quien diseña finalmente C apartir del B de Thompson, aportando un diseño de tipos de datos y estructuras de datos. Este por su puesto es un lenguaje que tiene como base una programación estructurada.

![c programa  ](C%20programa.jpg " Programa en c")
___
### TIPOS DE DATOS
* int

* float
* double
* char
* boll
____
### CONTROL DE FLUJOS 
* if else

* for (n)

* While (<>!= ==)
* beak 
* **swtich** en este especificamente se debe poner atención.
____
### Caracteristicas de C:
1. Programación estructurada (UNIX "ANSI C")

2. Lenguajes Naturales
3. Lenguaje de maquina *.exe "1001010010001"
____
## Creacción del Hello Word 
___
```c
#include <stdio.h> // llama a las librerias

//NOTAS
//1. Guardar :   ctrl s
//2. Compilar:  gcc src/main.c -o output/main.exe
//3. ejecutar:  ./output/main.exe
//4. script  :  main.c  	para    c 	 --> compilar se usa gcc 
//				main.cpp  	para	c++  --> compilar se usa g++

int main()
{
	printf("Hello pat_mic!\n");
	return (0);
} 
```
