# ESTRUCTURAS ITERATIVAS O CICLOS

Procesos que pueden ser repetitivos.  
Se cuenta con 3 estructuras principales que brindan soluciones repetitivas. Se las denomina **CICLOS**.

* **DO WHILE**
* **WHILE**
* **FOR**

La vida de un ciclo depende de una **condición** que indica si el ciclo se repite o se detiene. 
Toda estructura iterativa debe tener una condición de parada para que finalice, sino sería un ciclo infinito y podría dañar la máquina. 

CONSIDERACIONES:
 * Un ciclo se repite si la condición es TRUE;
 * Un ciclo termina si la condición es FALSE;
 * Corroborar que en algún momento la condición sea FALSE, para evitar el ciclo infinito.

  
  ## DO WHILE

  Primero se realizan una serie de acciones, y al finalizar se evalúa una condición, dependiendo si es T o F se realizará otra iteración, repitiendo los procesos que señalemos, o se rompe el ciclo.  

  Es decir que primero realizamos una serie de acciones, y luego colocamos la condición para considerar si queremos que se vuelva a repetir, o no. 


  **PSEUDOCODIGO**

  **DO**

  {

    Accion 1;
    Accion 2;
    ...
    Accion n;
  } 
  
  **WHILE** (condicion) 
 
 Ejemplo: algoritmo que repite los números del 1 al 10.

INICIO 

    entero i=1;

    do 
    {
        imprima "i";
        i++;
    }
    while(i<=10);

FIN  
 
## WHILE

Este cilco primero realiza una validación, y dependiendo del resultado (T/F) determina si ingresa al ciclo o no. Repite hasta que la condición falle. 

INICIO 

    entero i=1;
    
    while(i<=10){  
    imprima "i";  
    i++;  
    }

FIN  
 
## FOR

Es la abreviación de los 2 ciclos anteriores.
Adicional a la condición, también incluye la inicialización y el incremento.

INICIO 

    for(inicialización, condición, incremento)
    {
      Accion 1;
      Accion 2;
      ...
    }

FIN   

Una vez inicializado (se ejecuta 1 sola vez), luego se incrementa, se pregunta la condición, y se ejecutan las acciones. 
Luego se incrementa, se pregunta y segun se cumpla o no se sigue ejecutando.  
El ciclo FOR es como el ciclo MIENTRAS, primero pregunta y luego ejecuta.

 **PSEUDOCODIGO**

 INICIO 

    entero i;

    for(i=1; i<10; i++) 
    {
      imprima "i";
    }

FIN   

# COMPORTAMIENTO DE LOS CICLOS

**DO-WHILE** Lógica Ejecución-Condición
**WHILE** Lógica Condición-Ejecución
**FOR** Lógica Condición-Ejecución