# DO-WHILE
## EJERCICIO 1  

Algoritmo que imprima los primeros 10 números de la tabla del 2

INICIO  

    entero num, valor;
    valor=0;
    num=0;  

    do{
        valor = 2*num;
        imprima "2 * " + num + " = " + valor;
        num++;
    } while (num <= 10);

FIN

Lo mejor es tener en claro la condición básica del ciclo **DO - WHILE**

INICIO  

    entero counter = 0;
    do{

        cont++;
    } while (cont <10); 

FIN 

# WHILE
## EJERCICIO 1  

Algoritmo que imprima los primeros 10 números de la tabla del 2

INICIO  

    entero i=0;
    while(condicion){ 
            (logica aqui)

        i++;
        }
FIN 

INICIO  

    entero num, valor;
    num=0;
    valor=10;

    while(num<=10){ 
        valor = num*2;
        imprima "2 * " + num + " = " + valor;
        num++;
        }
FIN

# FOR
## EJERCICIO 1  

Algoritmo que recibe el sueldo de "n" personas y hs extras.
Debe imprimir el sueldo total de cada persona.  
Cada hs extra vale $3000.

INICIO  

    numerico sueldoBase, cantHsExt, sueldoTotal;
    numerico totalHsExt, cantPersonas, i;

    imprima "Ingrese la cantidad de personas";
    lea cantPersonas;

    for(i=0; i < cantPersonas; i++){

        imprima "Ingrese la información de la persona " + (i+1);

        imprima "Ingrese el sueldo base";
        lea sueldoBase;
        imprima "Ingrese cantidad de horas extras trabajadas";
        lea cantHsExt;

        totalHsExt = cantHsExt * 3000; 

        sueldoTotal = sueldoBase + totalHsExt;

        imprima "El sueldo total es " + sueldoTotal;

    }

FIN 


**ACLARACION**: 

El i++ dentro del ciclo for es incremento y asignación, por lo que modifica el valor de la variable.  
En cambio, el (i+1) imprime el resultado, pero no se lo pasa a ninguna variable.  
Al iniciar con la persona 1, e i=0; comenzará pidiendo los datos de la persona i+1 = 0+1 = 1. 

# MISMO EJERCICIO, COMPARADO A OTROS CICLOS

## WHILE

INICIO  

    numerico sueldoBase, cantHsExt, sueldoTotal;
    numerico totalHsExt, cantPersonas, i=0;  

    imprima "Ingrese la cantidad de personas";
    lea cantPersonas;

    while(i < cantPersonas){

        imprima "Ingrese la información de la persona " + (i+1);

        imprima "Ingrese el sueldo base";
        lea sueldoBase;
        imprima "Ingrese cantidad de horas extras trabajadas";
        lea cantHsExt;

        totalHsExt = cantHsExt * 3000; 

        sueldoTotal = sueldoBase + totalHsExt;

        imprima "El sueldo total es " + sueldoTotal;

        i++;

    }

FIN 

## DO-WHILE

INICIO  

    numerico sueldoBase, cantHsExt, sueldoTotal;
    numerico totalHsExt, cantPersonas, i=0;  

    imprima "Ingrese la cantidad de personas";
    lea cantPersonas;

    do{

        imprima "Ingrese la información de la persona " + (i+1);

        imprima "Ingrese el sueldo base";
        lea sueldoBase;
        imprima "Ingrese cantidad de horas extras trabajadas";
        lea cantHsExt;

        totalHsExt = cantHsExt * 3000; 

        sueldoTotal = sueldoBase + totalHsExt;

        imprima "El sueldo total es " + sueldoTotal;

        i++;

    } while(i < cantPersonas);

FIN 

# EJERCICIO CICLOS ANIDADOS

Algoritmo que muestre la tabla de multiplicar de los números del 1 al 10 

INICIO 

    entero i,j,valor;

    for (i=0; i<=10; i++) 
    {
        for(j=0; j<=10;j++)
        {
            valor=i*j;
            imprimir i + "*" + j + "=" + valor;
        }
    }

FIN 

INICIO 

    entero i,j,valor, tabla; max;

    imprima "Hasta qué tabla pretende multiplicar cada número?";
    lea tabla;
    imprima "Cuantos números desea multiplicar por cada tabla?";
    lea max;

    for (i=0; i<=tabla; i++) 
    {
        for(j=0; j<=max;j++)
        {
            valor=i*j;
            imprimir i + "*" + j + "=" + valor;
        }
    }

FIN 


**i** = representa la tabla de cada número. Ej: la tabla del 1, la tabla del 2... hasta la tabla del 10.
**j** = representa el número a multiplicar. 1***1**; 1***2**; etc. 