# ESTRUCTURAS CONDICIONALES

Las estructuras condicionales se utilizan para tomar decisiones lógicas.  
También llamadas estructuras de **decisión**. 
Se evalúa una condición y depende del resultado se define la acción a realizar (el flujo del programa/sistema). 

3 grupos de condiciones: 
* Condiciones Simples (sólo 1 camino por realizar si se cumple la condición. Sino el algoritmo continúa el flujo establecido)
* Condiciones Dobles (dos caminos a realizar, nunca ambos a la vez)
* Condiciones Múltiples (más de 2 caminos)

## CONDICIONES SIMPLES (IF)
Permite ejecutar 1 acción cuando se cumple 1 condición. 
 
```
    if (condición)  
        {  
            Acción 1,  
            Acción 2...  
        }  
```
 
 *Se muestra lo que está dentro del bloque de las {}, si la condición es V*

## CONDICIONES DOBLES (IF-ELSE) 

Permiten ejecutar determinada acción cuando se cumple una condición, pero en caso que la condición no se cumpla, ejecuta otro camino con acciones diferentes. 
 
 Condición = TRUE ==> Ejecuta acciones dentro del **if**  
 Condición = FALSE ==> Ejecuta accionesd entro del **else**

```  
 if (condición)  
    {  
        Acción 1;  
    }  
    else {   
        Acción 2;  
    }  
```       
 
**INICIO**   

    entero edad;   
    lea edad;
    if (edad >= 18)  
    {  
        imprima "Eres mayor de edad";  
    }  
    else {  
        imprima "Eres menor de edad";  
    }

**FIN** 

#### **NUNCA SE EJECUTAN AMBOS CAMINOS. O SE EJECUTA UNO, O EL OTRO** 
<br> 

## CONDICIONES MULTIPLES (IF - IF ELSE - ELSE) 
*  *Con condiciones anidadas*

Casos en los que después de tomar una decisión, se requiera seguir un posible camino donde se deban implementar nuevas condiciones.  
Para esto se aplican las condicionales, donde en cada bloque IF o ELSE pueden existir nuevas condiciones, y dentro de éstas nuevos procesos, y así sucesivamente.  
 
(Condiciones dentro de bloques de condiciones IF o de bloques ELSE)

*Se debe considerar que si el algoritmo utiliza muchas condiciones anidadas, el código puede resultar extenso y complejo.*

EJEMPLO = Algoritmo que determine si un número es +, - o cero.


INICIO   
```
    entero num;  
    lea num;  

    if (num <0) {  
        imprima "Negativo";  
    } else {  
        if (num > 0) {  
            imprima "Positivo";  
        } else {  
            imprima "Cero";  
        }  
    }
```
FIN   
 

 *  *Con bifurcaciones*

 Cuando se requieren varias condiciones, con anidadas puede resolverse.  
 Sin embargo, cuando hay una gran cantidad de condiciones, puede resultar complejo. En este caso es preferible utilizar la bifurcación. 

 La Bifurcación permite elegir un camino dependiendo de 1 condición, que recibe la estructura **SWITCH**.   
 La condición se evalúa, y depende de su contenido se elije el camino a seguir con las respectivas acciones.   

INICIO  
```
SWITCH (condicion) 
  
    {  
        CASO a:  
            Accion 1;  
        CASO b:  
            Accion 2;  
        CASO c:  
            Accion 3;  
        DEFAULT:  
            Accion n;  
    }

FIN 
```
  
Ejemplo: algoritmo que permita leer un número e imprimir el nombre correspondiente.  

CODIGO   ESTACION

1       INVIERNO  
2       VERANO  
3       OTOÑO  
4       PRIMAVERA  

INICIO

    entero estacion;
    lea estacion;
    switch(estacion) 
    {
        case 1: imprima "INVIERNO";
            break;  
        case 2: imprima "VERANO";
            break; 
        case 3: imprima "OTOÑO";
            break; 
        case 4: imprima "PRIMAVERA";
            break; 
        default: imprima "Estación incorrecta";
            break;
    }

FINAL