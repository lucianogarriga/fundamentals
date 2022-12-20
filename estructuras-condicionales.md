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
 
...
 if (condición)  
    {  
        Acción 1,  
        Acción 2...  
    }  
...
 
 *Se muestra lo que está dentro del bloque de las {}, si la condición es V*

## CONDICIONES DOBLES (IF-ELSE) 

Permiten ejecutar determinada acción cuando se cumple una condición, pero en caso que la condición no se cumpla, ejecuta otro camino con acciones diferentes. 
 
 Condición = TRUE ==> Ejecuta acciones dentro del **if**  
 Condición = FALSE ==> Ejecuta accionesd entro del **else**

...  
 if (condición)  
    {  
        Acción 1;  
    }  
    else {   
        Acción 2;  
    }  
...    

//   
//   
 
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

## CONDICIONES MULTIPLES (IF - IF ELSE - ELSE) 

Casos en los que después de tomar una decisión, se requiera seguir un posible camino donde se deban implementar nuevas condiciones.
Para esto se aplican las condicionales, donde en cada bloque IF o ELSE pueden existir nuevas condiciones, y dentro de éstas nuevos procesos, y así sucesivamente.  
 
(Condiciones dentro de bloques de condiciones IF o de bloques ELSE)

*Se debe considerar que si el algoritmo utiliza muchas condiciones anidadas, el código puede resultar extenso y complejo.*

EJEMPLO = Algoritmo que determine si un número es +, - o cero.

INICIO 
    entero num;
    lea num;
    **if**(num <0) {
        imprima "Negativo";
    } **else** {
        **if** (num > 0) {
            imprima "Positivo";
        } **else** {
            imprima "Cero";
        }
    }
FIN   




