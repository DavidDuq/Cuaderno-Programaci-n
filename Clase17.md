## CLASE 17 : **CORRECCIÓN DEL WORKSHOP**
___
**FECHA** :  20 DE DICIEMBRE DEL 2022
___
```c
#include <stdio.h>
#include <stdlib.h>

#define MAXTALLA 10
#define PI 3.14
int len = 0;

int getNumber(char label[])
{
    char numero[10];
    int n=0;
    do{
        printf("%s ", label);
        gets(numero);
        sscanf(numero,"%i \n", &n);
    }while (n <= 5);
    return n;
}
void DrawA(int tam, char caracter)
{
    for (int f = 0; f < tam; f++)
    {
        for (int c = 0; c < tam; c++)
            if (c==0 || f ==0 || tam/2==f || c ==(tam -1))
                printf("%c",caracter);
            else
                printf(" ",c);
        printf("\n"); 
    }
}
void DrawL(int tam, char caracter, char m[][len])
{
    for (int f = 0; f < tam; f++)
    {
        for (int c = 0; c < tam; c++)
            if (c==0 || f ==(tam -1))
                m[f][c]=caracter;   // printf("%c",caracter);
            else
                m[f][c]=' ';        // printf(" ",c);
        //printf("\n"); 
    }
}
void DrawE(int tam, char caracter, char m[][len])
{
    for (int f = 0; f < tam; f++)
    {
        for (int c = 0; c < tam; c++)
            if(f ==0 || c==0 || tam/2 == f || f== tam -1)
                m[f][c]= caracter; //printf("%c ",caracter);
            else
                m[f][c]=' '; //printf(" ");
        //printf("\n");
    }
}
void DrawO(int tam, char caracter, char m[][len])
{
    for (int f = 0; f < tam; f++)
    {
        for (int c = 0; c < tam; c++)
            if(f ==0 || c==0 || c== tam -1 || f== tam -1)
                m[f][c]= caracter;  // printf("%c ",caracter);
            else
                m[f][c]= ' ';  //printf("  ");
        //printf("\n");
    }
}

void main( )
{   //PI  = 3.1416;
    len = 12;
    len = getNumber("Ingresa un numeros mayor a 5 : ");
    char caracter = '+';
    char mL[len][len];
    char mE[len][len];
    char mO[len][len];

    DrawL(len, caracter, mL);
    DrawE(len, caracter, mE);
    DrawO(len, caracter, mO);

    system("clear");
    for (int f = 0; f < len; f++)
    {
        for (int c = 0; c < len; c++)
            printf("%c ",mL[f][c]);
        printf(" ");
       
        for (int c = 0; c < len; c++)
            printf("%c ",mE[f][c]);
        printf(" ");
        
        for (int c = 0; c < len; c++)
            printf("%c ",mO[f][c]);
        printf("\n");
    }
    system("pause");
}
```