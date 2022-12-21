# CONDICIONAL SIMPLE
## EJERCICIO 1  

Algoritmo que solicite un numero. Si es negativo, que lo convierta en positivo.

++ = +  
+- = -  
-- = +  
-+ = -

1ro -> Determinar la condicion
 -5 * -1 = +5

### **PSEUDOCODIGO**   
  
INICIO  

    entero num;  
    imprima "Ingrese el numero";  
    lea num;    
     
     if (num <0){
    num *= -1;
    } 
     
    imprima "El numero es: " + num;

FINAL

EJEMPLO:    

num = -2  
num <0 = true  
num = num *(-1)  
num = -2*(-1)  
num = 2

## EJERCICIO 2 

La tienda "Indumentaria La Seleccion" realiza 50% de descuento en compras mayores o iguales a $100.000.  
Hacer un algoritmo que permita validar cuando se debe aplicar el descuento.  
En caso que el descuento sea valido, se debe informar al ususario indicando el valor descontado. 

descuento 0.5  
compras >= 100000   
si se cumple la condicion, descuento = compra*0.5   
pagar = compra - descuento 
 
### **PSEUDOCODIGO**   
  
INICIO  

    numerico valorCompra, descuento, valorFinal;  
    imprima "Ingrese el valor de la compra";  
    lea valorCompra;  
    descuento = 0;  
    valorFinal = valorCompra;  
  
    if(valorCompra >= 100000){  
        descuento = valorCompra*0.5;  
        valorFinal = valorCompra - descuento;
        imprima "Se aplico un dto del 50% equivalente a: + descuento";
    }  

    imprima "El valor final es de " + valorFinal;  
FINAL  

# CONDICIONALES DOBLES
## EJERCICIO 1  

Algoritmo que solicite un numero, e indique si es + o -  

INIICIO

    entero num;
    imprima "Ingrese numero";
    lea num; 

    if(num <0){
        imprima "El numero es negativo";
    } else {
        imprima "El numero es positivo";
    } 
FINAL
 
## EJERCICIO 2  

La tienda "Indumentaria La Seleccion" realiza 50% de descuento en compras mayores o iguales a $100.000, sino un 10% en compras normales.  
Hacer un algoritmo que permita validar cuando se debe aplicar el descuento.  
En caso que el descuento sea valido, se debe informar al ususario indicando el valor descontado. 
 
### **PSEUDOCODIGO**   
  
INICIO  

    numerico valorCompra, descuento, valorFinal;  
    imprima "Ingrese el valor de la compra";  
    lea valorCompra;  
    descuento = 0;  
    valorFinal = valorCompra;  
  
    if(valorCompra >= 100000){  
        descuento = valorCompra*0.5;  
        valorFinal = valorCompra - descuento;
        imprima "Se aplico un dto del 50% equivalente a: + descuento";
    }  else {
        descuento = valorCompra*0.1;  
        valorFinal = valorCompra - descuento;
        imprima "Se aplico un dto del 10% equivalente a: + descuento";
    }

    imprima "El valor final es de " + valorFinal;  
FINAL

# CONDICIONALES MULTIPLES
## EJERCICIO 1  

Crear un algoritmo que lea 2 números y determine cual es mayor, cual menor o si son iguales.

INICIO  

    numerico num1, num2;  
    imprima "Ingrese el valor del numero 1";  
    lea num1;  
    imprima "Ingrese el valor del numero 2";  
    lea num2;  

    if(num1 < num2){
        imprima "Num1 es menor a num2";
    } else {
        if(num1 > num2){
            imprima "num1 es mayor a num2";
        } else {
            imprima "num1 es igual a num2";
        }
    }
FINAL  

## EJERCICIO 2

De un empleado se conoce su Sueldo y Antiguedad. Se debe crear un programa que lea los datos de entrada e informe:
* Si el sueldo es <500 y su antiguedad >=10 años, darle un aumento del 20%, y mostrar el sueldo a pagar;
* Si el sueldo <500 y antiguedad <10 años, darle un aumento 5%;
* Si el sueldo >=500, mostrar el sueldo sin cambios;

INICIO 
    numerico sueldo, antiguedad, aumento;
    texto mensaje="";
    imprima "Ingrese sueldo";
    lea sueldo;
    imprima "Ingrese antiguedad";
    lea antiguedad;
    aumento = 0;

    if(sueldo<500 && antiguedad >=10){
        aumento = sueldo*0.20;
        sueldo = sueldo + aumento;
        mensaje="Tiene un aumento del 20%, y el sueldo total es: " + sueldo;
    } else {
        if(sueldo <500 && antiguedad <10){
            aumento = sueldo*0.05;
            sueldo = sueldo + aumento;
            mensaje="Tiene un aumento del 5%, y el sueldo total es: " + sueldo;
        } else (sueldo >=500){
            mensaje="No tiene aumentos, y el sueldo es: " + sueldo;
        }
    
    imprima mensaje;
    }
FINAL