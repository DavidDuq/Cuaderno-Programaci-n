## CLASE 18: **ARCHIVOS**
___
**FECHA** : 3 DE ENERO DEL 2023 
___
### EJEMPLO 
___
```c
# incluir < iostream >
# include < fstream >  // flujo de información
utilizando el espacio de  nombres  estándar ;
void  leerArchivo (string archivo)
{
    int pagina = 1 ;
    cadena s;
    ifstream f (archivo);

    si (!f. está_abierto ())
        cerr<< " error al abrir el archivo. " <<endl;
    más
        hacer
        {
            obtener línea (f,s);
            cout<<s<<endl;
            si (pag++% 5 == 0 )
            obtener char ();
        } while (!f. eof ());
    F. cerrar ();    
}
int  principal (){
    leerArchivo ( " archivos \\ texto.txt " );
    devolver  0 ;
}
```