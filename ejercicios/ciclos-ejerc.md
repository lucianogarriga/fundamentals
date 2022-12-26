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

Algoritmo que imprima los primeros 10 números de la tabla del 2

INICIO  

    entero num, valor; 
    valor=0;

    for(entero num = 0; num <=10; num++)
    {
        valor = num * 2;
        imprima "2* " + num + " = " + valor;
    }
FIN 
