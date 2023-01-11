## CLASE 16: **REALIZACIÓN DEL WORKSHOP**
___
**FECHA** : 19 DE DICIEMBRE DEL 2022
____
## WORKSHOP GRUPO 1
___
| Actividad   | Puntaje     |  | TEMPORALIDAD |
|-------------|-------|-----|-----------------|
| Exámen      |  3          || BIMESTRAL      |
| Proyecto    |  3          || BIMESTRAL           |
| Workshop    |  2          || SEMANAL        |
| Tareas, Deberes      |  2          || SEMANAL        |
____
### DESARROLLO
___
```C
#include<stdio.h>
void MatrizLetraM(int nummatriz, char caracter){

    char Nombre[nummatriz][nummatriz];


        for(int i=0; i<nummatriz; i++){

            for(int j=0; j<nummatriz; j++){

                Nombre[i][j]= caracter;
            }
            }
            for(int i=0; i<nummatriz; i++){
                for(int j=0; j<nummatriz; j++){

                    if((j==0)||(j==nummatriz-1)||((i==j)&&(j<=nummatriz/2))||((i+j==nummatriz-1)&&(j>=nummatriz/2))||((nummatriz%2==0)&&(i+j==nummatriz-1)&&(j>=(nummatriz/2)-1))){

                         printf("%c  ", Nombre[i][j]);
                    }else
                       printf("   ");
            }
                printf("\n");
            }
}
void MatrizLetraK(int nummatriz, char caracter){

    char Nombre[nummatriz][nummatriz];

        for(int i=0; i<nummatriz; i++){

            for(int j=0; j<nummatriz; j++){

                Nombre[i][j]=caracter;
            }
            }
            for(int i=0; i<nummatriz; i++){

                for(int j=0; j<nummatriz; j++){

                    if((j==0)||(j==1)||((i+j==nummatriz-1)&&(j>=nummatriz/2))||((i==j)&&(j>=nummatriz/2)) ){

                         printf("%c  ", Nombre[i][j]);
                    }
                    else

                        printf("   ");
            }
                printf("\n");
            }
}

void MatrizLetraN(int nummatriz, char caracter){
    char Nombre[nummatriz][nummatriz];
        for(int i=0; i<nummatriz; i++){
            for(int j=0; j<nummatriz; j++){
                Nombre[i][j]=caracter;

            }

            }

            for(int i=0; i<nummatriz; i++){

                for(int j=0; j<nummatriz; j++){

                     

                    if((j==0)||(j==nummatriz-1)||(i==j)){

                         printf("%c  ", Nombre[i][j]);

                   

                    }

                    else

                        printf("   ");

            }

                printf("\n");

            }

     



}



void MatrizLetraJ(int nummatriz, char caracter){

    char Nombre[nummatriz][nummatriz];



        for(int i=0; i<nummatriz; i++){

            for(int j=0; j<nummatriz; j++){

                Nombre[i][j]=caracter;

            }

            }



            for(int i=0; i<nummatriz; i++){

                for(int j=0; j<nummatriz; j++){

                     

                    if((i==0)||((i==nummatriz-1)&&(j<nummatriz/2))||(j==nummatriz/2)){

                         printf("%c  ", Nombre[i][j]);

                   

                    }

                    else

                        printf("   ");

            }

                printf("\n");

            }

     
}


void MatrizLetraG(int nummatriz, char caracter){
    char Nombre[nummatriz][nummatriz];

        for(int i=0; i<nummatriz; i++){
            for(int j=0; j<nummatriz; j++){
                Nombre[i][j]=caracter;
            }
            }

            for(int i=0; i<nummatriz; i++){
                for(int j=0; j<nummatriz; j++){
                     
                    if((i==0)||(j==0)||(i==nummatriz-1)||((j==nummatriz-1)&&(i>=nummatriz/2))||((i==nummatriz/2)&&(j>=nummatriz/2))){
                         printf("%c  ", Nombre[i][j]);
                    
                    }
                    else
                        printf("   ");
            }
                printf("\n");
            }
      

}

int main(void){

char nomb1 [50];

 char nomb2 [50];

 char nomb3 [50];

 char nomb4 [50];

 char nomb5 [50];

 char nomb6 [50];

 char nomb7 [50];

 char nomb8 [50];
 int tamano =0;
 char caracter;

 printf("Nombre y apellido Persona 1: "); gets(nomb1);

 printf("Nombre y apellido Persona 2: "); gets(nomb2);

 printf("Nombre y apellido Persona 3: "); gets(nomb3);

 printf("Nombre y apellido Persona 4: "); gets(nomb4);

 printf("Nombre y apellido Persona 5: "); gets(nomb5);

 printf("Nombre y apellido Persona 6: "); gets(nomb6);

 printf("Nombre y apellido Persona 7: "); gets(nomb7);

 printf("Nombre y apellido Persona 8: "); gets(nomb8);

printf("\n\nDigite el caracter que desea imprimir: "); scanf("%c", &caracter);

printf("\n\nDigite el tamano de su letra: "); scanf("%i", &tamano);

while(tamano<6){



    printf("No es el tamano indicado: "); scanf("%i", &tamano);



}
    printf("\n\n\n");

    MatrizLetraG(tamano, caracter);


    printf("\n\n\n");

    MatrizLetraJ(tamano, caracter);
    
    printf("\n\n\n");

    MatrizLetraK(tamano, caracter);

    printf("\n\n\n");

    MatrizLetraM(tamano, caracter);

    printf("\n\n\n");

    MatrizLetraN(tamano, caracter);

    printf("\n\n\n");
}
```