## EJERCICIO 1

Algoritmo que lea tres notas y calcule e imprima el promedio
datos de entrada para el algoritmo. 

El usuario ingresara tres notas y el programa los leerá. 

Planteo - análisis - diseño - codificación 



### **PSEUDOCODIGO**   
  
INICIO  

    numerico nota1, nota2, nota3, prom;  
    imprima "Porfavor ingrese las notas";  
    lea nota1;  
    lea nota2;  
    lea nota3;  

    prom = (nota1+nota2+nota3) /3;
FINAL


## **EJERCICIO 2**
 
Algoritmo que reciba como entrada el sueldo de una persona y sus horas extras trabajadas. 
Luego que imprima el sueldo total. 
Cada hora extra vale $3000.  


sueldoBase = 100.000   
cantHorasExt = 2 

totalExtras = cantHorasExt * 3000 

sueldoTotal = sueldoBase + totalExtras 
 
 ### **PSEUDOCODIGO** 


 INICIO   

    numerico sueldoBase, cantHorasExt, totalExtras, sueldoTotal;

    imprima "Ingrese el sueldo base";
    lea sueldoBase;
    imprima "Ingrese la cantidad de horas extras trabajadas";
    lea cantHorasExt;
     
    totalExtras = cantHorasExtras * 3000; 

    sueldoTotal = sueldoBase + totalExtras;

    imprima "El sueldo total es = " + sueldoTotal;

FINAL 

## **EJERCICIO 3**
 
Algoritmo que calcule lo que gana un empleado en base a las horas trabajadas. 
Cada hora se paga 2000. 
Adicionalmente se le realizan descuentos relativo a un impuesto de seguridad del 10% de su sueldo. 

El sistema debe imprimir un mensaje indicando el nombre del empleado y su sueldo total.    

sueldoNeto   
sueldoBruto = cantHoras*2000  
impuesto = sueldoBruto*(10/100)  
sueldoNeto = sueldoBruto - impuesto  

### **PSEUDOCODIGO**
 
INICIO  
 
    texto nombre;
    numerico cantHoras, impuesto, sueldoBruto, sueldoNeto;  

    imprima "Ingrese nombre empleado";
    lea nombre;

    imprima "Ingrese cantidad de horas trabajadas";
    lea cantHoras; 

    sueldoBruto = cantHoras*2000;
    impuesto = sueldoBruto*0.10;
    sueldoNeto = sueldoBruto-impuesto; 
 
    imprima "El empleado " + nombre + "cobrará un sueldo de: " + sueldoNeto; 
    
FIN
