## CLASE 13 : **ARRAYS-PROCEDIMIENTOS Y FUNCIONES**
___
**FECHA** : 12 DE DICIEMBRE DEL 2022 
___
>En esta clase se presento un ejemplo
```C
#include <stdio.h>
#include <string.h>

int suma();
int sumaInt(int a, int b);
void showConsola(int rta);
float sumafloat(float a, float b);
int sumaFantasma();

int ValidarClave(char clave[])
{
	char claveSecreta = "1234231";
	if(strcmp(clave, claveSecreta )==0)
		return 1;
	return 0;
}

void ValidarClaveArray( )
{
	char contrasena[]="pato";
	char clave[]="pat1";
	int validador=1;
	for (int i = 0; i < sizeof(clave); i++)
		if (clave[i]!=contrasena[i])
			validador= 0;
	
	if(validador ==1)
		printf("clave correcta \n\n");
	else
		printf("clave incorrecta \n\n");

}

int main()
{

	//ValidarClaveArray( );

	char key[]="1234231";
	if(ValidarClave(key)==0)
		printf("clave  correcta \n\n");
	else
		printf("clave  incorrecta \n\n");

	////////////////////////////////////////
	int rta = suma();
	printf("La suma es: %i \n", rta  );

	rta = sumaInt(5,8);
	printf("La suma es: %i \n", rta  );

	printf("La suma es: %.2f \n", sumafloat(5.5,8.12354)  );

	showConsola(sumaInt(5,8));
	
	return (0);
}

//procedimiento
void showConsola(int rta)
{
	printf("La suma es: %i \n", rta  );
}

//función
int suma()
{
	int a =10,b=20, r =0;
	r= a+b;
	return r;
}
int sumaInt(int a, int b)
{
	return a+b;
}
float sumafloat(float a, float b)
{
	return a+b;
}
```