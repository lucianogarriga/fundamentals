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

	public static void main (String[] args) {
		
		double valorCompra=0,descuento=0,valorFinal=0;
		String mensajeDto="",mensaje="";
		
		valorCompra=Double.parseDouble(JOptionPane.showInputDialog(
				"Ingrese valor de la compra"));

        //También podría ser declarado como un número entero
        //int valorCompra=0;
        //valorCompra=Integer.parseInt(JOptionPane.showInputDialog(""));
		
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

## **EJERCICIO 4 - ESTRUCTURA CONDICIONAL DOBLE**
### Una tienda realiza descuento del 50% en compras + o = a $100.000, y un descuento del 10% en compras menores a dicho monto. Hacer un algoritmo que permita validar cuando se den las condiciones para aplicar un descuento. En caso que el descuento sea valido, que informe al usuario indicando el valor descontado.
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
    }  else {
        descuento = valorCompra*0.1;
        valorFinal = valorCompra - descuento;
        imprima "Se aplico un dto del 10% equivalente a: + descuento";
    }

    imprima "El valor final es de " + valorFinal;  

FINAL  

<br>

> ### **RESOLUCION EJERCICIO 4 EN ARCHIVO . JAVA**
<br>

```java
package condiciones;

import javax.swing.JOptionPane;

public class EjercicioCondicionalDoble {

	public static void main (String[] args) {
		
		double valorCompra=0,descuento=0,valorFinal=0;
		String mensajeDto="",mensaje="";
		
		valorCompra=Double.parseDouble(JOptionPane.showInputDialog(
				"Ingrese valor de la compra"));
		
		if(valorCompra >= 100000) {
			descuento=valorCompra*0.5;
			valorFinal=valorCompra-descuento;
			mensajeDto="Se realizó un descuento del 50% "
					+ "equivalente a " + descuento;
			System.out.println(mensajeDto);
			JOptionPane.showMessageDialog(null,mensajeDto);
		} else {
			descuento=valorCompra*0.1;
			valorFinal=valorCompra-descuento;
			mensajeDto="Se realizó un descuento del 10% "
					+ "equivalente a " + descuento;
			System.out.println(mensajeDto);
			JOptionPane.showMessageDialog(null,mensajeDto);
		}
		
		mensaje="El valor total a pagar es: " + valorFinal;
		System.out.println(mensaje);
		JOptionPane.showMessageDialog(null,mensaje);
	}
}
```

## **EJERCICIO 5 - ESTRUCTURA CONDICIONAL MULTIPLE**
### Algoritmo que solicite un codigo y que imprima el dia correspondiente
### 1. Lunes 2. Martes 3. Miercoles 4. Jueves 5. Viernes 6. Sabado 7. Domingo
<br> 

```java

package condiciones;

import javax.swing.JOptionPane;

public class EjercicioCondMultiple {

	public static void main(String[]args) {
		int codigo=0;
		String mensaje="MENU\n\n";
		
		mensaje+="1. Lunes\n";
		mensaje+="2. Martes\n";
		mensaje+="3. Miercoles\n";
		mensaje+="4. Jueves\n";
		mensaje+="5. Viernes\n";
		mensaje+="6. Sabado\n";
		mensaje+="7. Domingo\n";
		
		codigo=Integer.parseInt(JOptionPane.showInputDialog(mensaje+"\n Ingrese el código"));
	
		switch (codigo) {
		case 1: JOptionPane.showMessageDialog(null,"El día es Lunes");
			break;
		case 2: JOptionPane.showMessageDialog(null,"El día es Martes");
			break;
		case 3: JOptionPane.showMessageDialog(null,"El día es Miercoles");
			break;
		case 4: JOptionPane.showMessageDialog(null,"El día es Jueves");
			break;
		case 5: JOptionPane.showMessageDialog(null,"El día es Viernes");
			break;
		case 6: JOptionPane.showMessageDialog(null,"El día es Sabado");
			break;
		case 7: JOptionPane.showMessageDialog(null,"El día es Domingo");
			break;

		default: JOptionPane.showMessageDialog(null,"El código no existe");
			break;
		}
		
	}
	
}
```

## **EJERCICIO 6 - CICLO FOR**

```java

package condiciones;

import javax.swing.JOptionPane;

public class EjercicioCicloFor {

	public static void main(String[]args) {
		int i, suma = 0, cant=0;

        cant=Integer.parseInt(JOptionPane.showInputDialog("Ingrese la cantidad"));

        for (i=0; i<=cant;i++){
            suma=suma+i;
        }

        System.out.prinln("La suma de los " +cant+" primeros numeros es: " +suma);
	}
	
}
```

## **EJERCICIO 7 - CICLOS DO-WHILE ANIDADOS**

### Algoritmo que imprima la suma de los 10 primeros numeros, usando el ciclo do-while, y lo repita la cantidad de veces que el usuario desee.
<br>

```java
    package condiciones;

    import javax.swing.JOptionPane;

    public class EjercicioCicloAnidado1 {

        public static void main(String[]args) {
            int i=0,j=0, suma = 0, cant=0, n=0;

            n=Integer.parseInt(JOptionPane.showInputDialog("Ingrese la cantidad de veces a repetir"));

            do{
                //
                JOptionPane.showInputDialog(null,"Inicia la sumatoria");
                cant=Integer.parseInt(JOptionPane.showInputDialog("Ingrese la cantidad de numeros a sumar"));
                //cada vez que empecemos nuestro algoritmo, hay que reiniciar las variables
                i=0;
                suma=0;
                do{
                    suma=suma+i;
                    i++;
                } while(i<=cant);

                System.out.prinln("La suma de los " +cant+" primeros numeros es: " +suma);
                //

                j++;
            }while(j<n);


        }
        
    }
```

## **EJERCICIO 8 - CICLOS WHILE ANIDADOS**

### Algoritmo que imprima la suma de los 10 primeros numeros, usando el ciclo while, y lo repita la cantidad de veces que el usuario desee.
<br>

```java
    package condiciones;

    import javax.swing.JOptionPane;

    public class EjercicioWhileAnidado {

        public static void main (String[]args) {
            int i, suma, cant=0;
            String resp="si";
            
            do {
                //
                cant=Integer.parseInt(JOptionPane.showInputDialog("Ingrese "
                        + "la cantidad"));
                i=0;
                suma=0;
                while(i<=cant) {
                    suma=suma+i;
                    i++;
                }
                System.out.println("La suma de los "+cant+" primeros numeros es "+suma);
                //
                resp=JOptionPane.showInputDialog("Ingrese si, si desea continuar");
                
            } while (resp.equals("si"));
            //Para comparar palabras que ingrese el usuario.
            //resp no solo es una variable, sino que a la vez es un Objeto
            //por ende, no se puede hacer la comparación == como se hace
            //con variables normales, porque es un Objeto también.
            
        }
        
    }
```
## **EJERCICIO INTEGRADOR**

### Un agricultor desea saber el costo de producción de un cultivo de acuerdo a la semilla, conociendo el numero de semillas que utilizara y el costo de cada una. 
|Verdura | Tipo | Valor x semilla |
|----------|--------------|---------|
|Tomate|Chonto|15|
||Ensalada|20| 
|Repollo||10|
|Papa| Criolla |8|
||Pastusa|9|
||Salentuna|11|
|Cebolla|Larga|15|
||De huevo|13|    

Dependiendo del tipo de semilla que tiene que sembrar, se deberá desplegar un menú y en base a ello se realizarán los cálculos. 

costoSemillas = numeroSemillas x valorSemilla 

> ### RESOLUCION EJERCICIO INTEGRADOR 

```java

package bonus;

import javax.swing.JOptionPane;

public class bonus {
	
	public static void main(String[]args) {
		String menuVerdura,menuTomate,menuPapa,menuCebolla;
		int codigoVerdura, codigoTipo, valorSemilla=0, numeroSemilla, costoSemilla;
		String verdura="", tipo="", resp="";
		boolean error=false;
		
		do{
			//
			error=false;
			
			menuVerdura="MENU VERDURA\n\n";
			menuVerdura+="1. Tomate\n";
			menuVerdura+="2. Repollo\n";
			menuVerdura+="3. Papa\n";
			menuVerdura+="4. Cebolla\n\n";
			
			menuTomate="TIPO TOMATE\n\n";
			menuTomate+="1. Chonto\n";
			menuTomate+="2. Ensalada\n\n";
			
			menuPapa="TIPO PAPA\n\n";
			menuPapa+="1. Criolla\n";
			menuPapa+="2. Pastusa\n";
			menuPapa+="3. Salentusa\n\n";
			
			menuCebolla="TIPO CEBOLLA\n\n";
			menuCebolla+="1. Larga\n";
			menuCebolla+="2. De huevo\n\n";
			
			codigoVerdura=Integer.parseInt(JOptionPane.
					showInputDialog(menuVerdura+" Ingrese el código de la verdura"));
		
			switch (codigoVerdura) {
			case 1: verdura="Tomate";
			
				codigoTipo=Integer.parseInt(JOptionPane.
				showInputDialog(menuTomate+" Ingrese el tipo de tomate"));
				
				switch (codigoTipo) {
				case 1: tipo="Chonto";
						valorSemilla=15;	
						System.out.println(tipo + " es el tipo elegido y cada semilla vale " + valorSemilla);
					break;
				case 2: tipo="Ensalada";
						valorSemilla=20;
						System.out.println(tipo + " es el tipo elegido y cada semilla vale " + valorSemilla);
				break; 
				default: error=true; 
					System.out.println("El tipo ingresado no existe");
					break;
				}
			
				break;
			case 2: verdura="Repollo";
					tipo="Normal";
					valorSemilla=10;
					System.out.println(tipo + " es el tipo elegido y cada semilla vale " + valorSemilla);	
				break;
			case 3: verdura="Papa";
			
				codigoTipo=Integer.parseInt(JOptionPane.
				showInputDialog(menuPapa+" Ingrese el tipo de papa"));
				
				switch (codigoTipo) {
				case 1: tipo="Criolla";
						valorSemilla=8;
						System.out.println(tipo + " es el tipo elegido y cada semilla vale " + valorSemilla);	
					break;
				case 2:tipo="Pastusa";
						valorSemilla=9;
						System.out.println(tipo + " es el tipo elegido y cada semilla vale " + valorSemilla);
					break;
				case 3:tipo="Salentuna";
						valorSemilla=11;
						System.out.println(tipo + " es el tipo elegido y cada semilla vale " + valorSemilla);	
					break;
				default: error=true; 
				System.out.println("El tipo ingresado no existe");
					break;
				}
			
				break;
			case 4: verdura="Cebolla";
			
				codigoTipo=Integer.parseInt(JOptionPane.
				showInputDialog(menuCebolla+" Ingrese el tipo de cebolla"));
				
				switch (codigoTipo) {
				case 1: tipo="Larga";
						valorSemilla=15;
						System.out.println(tipo + " es el tipo elegido y cada semilla vale " + valorSemilla);
					break;
				case 2: tipo="De huevo";
						valorSemilla=13;
						System.out.println(tipo + " es el tipo elegido y cada semilla vale " + valorSemilla);				
					break;
				default: error=true; 
				 System.out.println("El tipo ingresado no existe");
					break;
				}
			
				break; 

			default: error=true; 
			 System.out.println("El tipo de verdura no existe");
				break;
			}
			
			if (error==false) {
				
				numeroSemilla=Integer.parseInt(JOptionPane.
						showInputDialog("Ingrese la cantidad de semillas"));
				
				costoSemilla=numeroSemilla*valorSemilla;
				
				System.out.println("Verdura: " + verdura + " de tipo: " + tipo);
				System.out.println("Cantidad de semillas: " + numeroSemilla);
				System.out.println("Costo total de semillas: " + costoSemilla);	
				
			} else {
				System.out.println("Error en el ingreso de datos");
			}
						
			//
			System.out.println();
			System.out.println("**********************");
			System.out.println();
			
			resp=JOptionPane.showInputDialog("Ingrese 'si' si desea continuar");
		} while(resp.equalsIgnoreCase("si"));
		
	}
}
```