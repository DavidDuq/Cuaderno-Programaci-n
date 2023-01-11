## CLASE 10 : **FUNCIONES Y PROCEDIMIENTOS**
___
**FECHA** : 07 DE DICIEMBRE DEL 2022
___
## FUNCIONES
* Las funciones pueden residir en uno o varios ficheros fuente

* Una de esas funciones se llama main y es la primera en ejecutarse
* Un programa e C es una colección de funciones.
* Cada función tiene la forma
~~~ 
 tipo de dato nombre funcion   (declaraciones argumentos)
  {
  declaraciones y sentencias
  }
~~~
* En cambio cuando no lleve parámetros o ningun valor se le usa el termino **Void** *void funcion_(void)*
```c
#include <stdio.h>

#include <stdio.h>
// función : Tipo de Dato (no void) -> int, float, loble long, short,  ......  [return]
int Suma()
{
    int n1, n2, rta;
    n1 = 10;
    n2 = 23;
    rta = n1 + n2;
    return rta;
}

// función + parametros
int SumaPara(int n1, int n2)
{
    int rta;
    rta = n1 + n2;
    return rta;
}
// función que suma numeros enteros
int SumaParaShort(int n1, int n2)
{
    // forma corta de sumar sin variables
    return n1 + n2;
}

void main( )
{
    int rta = 0;
    rta = Suma();
    printf("\n La suma es: %d", rta);

    printf("\n ----------------- \n");

    rta = SumaPara(42,52);
    printf("\n La suma es: %d", rta);
   
    printf("\n ----------------- \n");
    printf("\n La suma es: %d", SumaParaShort(42,52) );
}
``` 