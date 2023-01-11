## CLASE 9 : **BUCLES**
___
**FECHA** : 6 DE DICIEMBRE DEL 2022
___
### CODIFICACIÓN DE ALGORITMIA
___
```c
#include <stdio.h>
int main()
{   //declarar e inicializar las variables
    int logitud =0, ancho=0, areaRect =0;
    
    printf("\n << Calula el area de un rectangulo >> \n ");
    printf("Ingrese la Logitud: ");
    scanf("%i", &logitud);

    printf("Ingrese la ancho: ");
    scanf("%i", &ancho);

    areaRect = logitud * ancho;

    printf("EL el area del rectangulo es: %i \n",areaRect);
    printf("EL el area del rectangulo de ancho %i y longitud %i es %i \n",ancho, logitud, areaRect);

    return 0;
}
```
___
### BUCLE CUADRADO FOR 
```c
#include <stdio.h>
 
int main()
{
 
    int num, a, b;
 
    printf("Numero de signos para el cuadrado:");
    scanf("%d",&num);
 
    for(b=1; b <= num; b++)
    {
        for(a=1; a<= num; a++)
        {
            if(b==1 || b== num)
            {
                if (a%2==0)
                printf("+ ");
                else
                printf("- ");
                
            }else if(a==1 || a== num){
                if (b%2==0)
                    printf("+ ");
                else
                    printf("- ");
            }else{
 
                printf("  ");
            }
        }
        printf("\n");
    }
}
```

### BUCLE DE ESCALERA FOR 
---

```c
int main(void)
{
    int nivel=5;
    
    for (int i = 0; i < nivel*2; i++)
    {
        if (i%2==0)
        {
            printf("__\n");
        }
        else
        {
            for (int f = 0; f <= i; f++)
                printf(" ");
            printf("|");        
        }
    }
     printf("\n\n");
    return 0;
}
```