# EJERCICIOS EN JAVA

## **EJERCICIO 1**
### Algoritmo que lea 3 notas y calcule e imprima el promedio.  

<br> 

### **PSEUDOCODIGO**

INICIO 
 
    numerico nota1,nota2,nota3,prom;  
    imprima "Por favor ingrese las notas";  
    lea nota1;  
    lea nota2;  
    lea nota3;

    prom=(nota1+nota2+nota3)/3;

    imprima "El promedio de las notas es: "+ prom;

FINAL

<br> 

> ### **RESOLUCION EJERCICIO 1 EN ARCHIVO . JAVA**
<br> 

```java
    import javax.swing.JOptionPane;

    public class EjercicioSecuencial {
        
        public static void main (String arg[] ) {

            double nota1,nota2,nota3,prom;
            
            nota1=Double.parseDouble(JOptionPane.showInputDialog("Ingrese nota 1"));
            nota2=Double.parseDouble(JOptionPane.showInputDialog("Ingrese nota 2"));
            nota3=Double.parseDouble(JOptionPane.showInputDialog("Ingrese nota 3"));
                    
            prom=(nota1+nota2+nota3)/3;
            
            System.out.println("El promedio es: " +prom);
            JOptionPane.showMessageDialog(null, "El promedio es: " +prom);
            
        }
    }
```

## **EJERCICIO 2**
### Algoritmo que reciba como entrada el sueldo de una persona y sus horas extras trabajadas. Luego imprima Sueldo Total.  Cada hora extra vale $3000. 
<br> 

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

<br> 

> ### **RESOLUCION EJERCICIO 2 EN ARCHIVO . JAVA**
<br> 

```java
    import javax.swing.JOptionPane;

    public class Ejercicio2Secuencial {
        
        public static void main (String arg[]) {
            double sueldoBase,cantHorasExtras,sueldoTotal,totalHorasExtras;
            
            sueldoBase=Double.parseDouble(JOptionPane.showInputDialog("Ingrese el sueldo base"));
            cantHorasExtras=Double.parseDouble(JOptionPane.showInputDialog("Ingrese la cantidad de horas extras"));
            
            totalHorasExtras=cantHorasExtras*3000;
            
            sueldoTotal=sueldoBase+totalHorasExtras;
            
            System.out.println("El sueldo total es: " +sueldoTotal);
            JOptionPane.showMessageDialog(null, "El sueldo total es: " +sueldoTotal);
        }
    }
    
``` 


## **EJERCICIO 3 - ESTRUCTURA CONDICIONAL SIMPLE**
### Una tienda realiza descuento del 50% en compras + o = a $100.000. Hacer un algoritmo que permita validar cuando se den las condiciones para aplicar un descuento. En caso que el descuento sea valido, que informe al usuario indicando el valor descontado.
<br> 

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

---
<br>
En Java, al trabajar variables dentro de métodos **se las debe inicializar** (public static void main {} es un método clásico de Java). Si queremos utilizarlas sin haberlas inicializado, el sistema arrojará un error. 
Una buena práctica es inicializar:    

<br> 

* Los datos numéricos en cero (0)  
    ```java
            {  
                double valorCompra = 0;  
            } 
    ```

* Los datos tipo string en una cadena vacía 
    ```java
            {  
                String mensaje="";  
            }
    ```
<br>

> ### **RESOLUCION EJERCICIO 3 EN ARCHIVO . JAVA**
<br>

```java
package condiciones;

import javax.swing.JOptionPane;

public class EjercicioCondicionalSimple {

	/*
	 * Una tienda realiza descuento del 50% en compras + o = a $100.000.
	 * Hacer un algoritmo que permita validar cuando se den las condiciones
	 *  para aplicar un descuento. En caso que el descuento sea valido,
	 *  se informe al usuario indicando el valor descontado.
	 */
	
	public static void main (String[] args) {
		
		double valorCompra=0,descuento=0,valorFinal=0;
		String mensajeDto="",mensaje="";
		
		valorCompra=Double.parseDouble(JOptionPane.showInputDialog(
				"Ingrese valor de la compra"));
		
		if(valorCompra >= 100000) {
			descuento=valorCompra*0.5;
			valorFinal=valorCompra-descuento;
			mensajeDto="Se realizó un descuento del 50% equivalente a " + descuento;

			System.out.println(mensajeDto);
			JOptionPane.showMessageDialog(null,mensajeDto);
		}
		
		mensaje="El valor total a pagar es: " + valorFinal;
		System.out.println(mensaje);
		JOptionPane.showMessageDialog(null,mensaje);
	}
}
```

