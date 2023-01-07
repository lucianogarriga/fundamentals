# JAVA

- Es un lenguaje de programación orientado a objetos (POO).  
Todo lo que se trabaja en el lenguaje se debe pensar como objetos.
- Independiente de la Plataforma (Multiplataforma)  
Se puede trabajar desde windows, mac, linux, etc.
- Es un Lenguaje Interpretado   
El intérprete convierte el código java a código de máquina (JVM - Java Virtual Machine)

### **TECNOLOGIAS JAVA**  '


**JME (JAVA MICRO EDITION)**   
Aplicaciones móviles.  
**JSE (JAVA STANDARD EDITION)**    
Aplicaciones de escritorio (stand alone), applets, etc.  
**JEE (JAVA ENTERPRISE EDITION)**  
Aplicaciones empresariales (web), entorno cliente-servidor, software distribuido,etc. 

### **JDK (JAVA DEVELOPMENT KIT)**
Es el software requerido para la creación de programas Java.  
Consiste en un conjunto de librerías y herramientas de desarrollo necesarias para los procesos de compilación y ejecución de las aplicaciones. 
Este a su vez trae dentro JRE.
Con JDK programo y ejecuto. 
Pero si vamos a instalar el software de un cliente, solo JRE que permite ejecutar.

### **JRE (JAVA RUNTIME ENVIRONMENT)**
Es el entorno mínimo para la ejecución de programas. Sin estas, las aplicaciones Java no podrían ser ejecutadas satisfactoriamente. 

### **ENTORNO DE DESARROLLO (IDE)**
Luego del proceso de instalación, podemos trabajar con Java desde diversos editores de texto almacenando el archivo con la extensión **.java**. 
Sin embargo, se debe usar un IDE para sacarle más provecho al lenguaje.  

- ECLIPSE
- NETBEANS
- INTELLIJ IDEA
- ORACLE JDEVELOPER 

## ESTRUCTURA DE UNA CLASE

Una clase equivale al archivo que contiene el código fuente de nuestro sistema. 
Un proyecto Java se puede componer de 1 o más clases. 
Deben tener un nombre igual al del archivo. 

## CONVENCIONES CLASES E INTERFACES

- La primera letra debe ser en Mayúscula
- Utiliza nomenclatura CamelCase
- Para Clases = los nombres deben ser SUSTANTIVOS (Sujeto) y van después de la palabra reservada **class**
- Para las *Interfaces* los nombres deben ser ADJETIVOS (califica el sustantivo) y van después de la palabra reservada **interface**

Ejemplos:

*class Persona  
class ClasePersona  
interface ActionListener*

El nombre de la clase debe coincidir con el nombre del archivo **.java**

Ejemplo:   
archivo => ClasePrincipal.java 

    public class ClasePrincipal {

    }

Esta clase tiene un indicador de que ha sido declarada como **publica**
 
    interface ClaseDosInterface {

    }

## PAQUETES

Por convención, llevan todo el nombre en minúsculas. 
Para utilizarlos, deben estar precedidos por la palabra **package**

*package paquete*;

Para poder utilizar los paquetes, las clases deben estar guardadas dentro de aquellos. 

## METODOS

Convenciones: comienzan en minúsculas y utilizan camelCase. 
Una estructura sería:

    public void metodo(){

    }
    public void metodoDos(){

    }

### VARIABLES

Convenciones para variables: 
- Debe contener el nombre, luego de definir el tipo de dato.
- Los nombres de los paquetes, metodos, variables, clases: deben ser **representativos**
- También comienzan en minúsculas e implementan camelCase.


**int** variablePrueba; 

### CONSTANTES

Almacenan información pero de manera inmutable, su valor no puede cambiar posteriormente.
Las convenciones establecen que los nombres de las constantes deben estar en **MAYÚSCULAS**.
Además, al comienzo de la definición de la constante lleva la palabra reservada **final**, lo que indica que no es una variable; luego lleva el tipo de dato (*int* por ejemplo), y luego el nombre de la constante.

Ejemplo:

**final int** PRECIO = 14;


# ECLIPSE IDE 

Para iniciar un proyecto **.java**, se comienza de la siguiente manera:

public class Principal {

    public static void main (String arg[]){
        //código fuente
    }

} 

Obligatoriamente debe iniciar de esa manera para que pueda leer nuestros algoritmos.  
El nombre del archivo (en este caso **Principal.java**) debe coincidir y ser igual al nombre de la class (**Principal**).  
Un proyecyo Java SE debe tener sólo un método *main* que inicia el sistema.  
Sin embargo, a modo de prácticas se pueden crear muchas clases independientes con su propio método main.

# NETBEANS IDE

Luego, creamos un proyecto en NetBeans IDE - **Java Application**.  
Luego dentro de NetBeans y la aplicación ya creada, damos click derecho a la carpeta "Source Packages" y creamos una nueva **clase**.  
De esta manera, nos queda el código fuente listo, al igual como nos manejamos en Eclipse IDE.

Entre estos dos, cambian algunas cosas como las formas de ejecutar el programa, o cómo lo visualizamos, pero el lenguaje es el mismo. 

Como hemos visto antes, primero se declara el tipo de dato y luego el nombre de la variable. 

**int**: número entero
**double**: número decimal

import javax.swing.JOptionPane;

public class Aplication {
	
	public static void main (String arg[] ) {

		String nombre;
		int edad;
		double num1,num2;
		String mensaje;
		
		nombre=JOptionPane.showInputDialog("Ingrese su nombre");
		edad=Integer.parseInt(JOptionPane.showInputDialog("Ingrese su edad"));
> Una **clase** - Por medio de un **método** - Recibe un **mensaje** que le estamos enviando

		num1=Double.parseDouble(JOptionPane.showInputDialog("Ingrese el número 1"));
		num2=Double.parseDouble(JOptionPane.showInputDialog("Ingrese el número 2"));
		
		double suma= num1+num2;
		
		mensaje="Su nombre es: "+ nombre + "\n";
		mensaje+="Su edad es: "+ edad + "\n";
		mensaje+="Num1= "+num1+", Num2= "+num2 + "\n";
		mensaje+="La suma es: " + suma + "\n";
		
		JOptionPane.showMessageDialog(null, mensaje);
		
		System.out.println(mensaje);
> Con este comando imprime el mensaje final por consola
		 
	}
}

El comando para imprimir un mensaje por consola es:

		System.out.print("Hola, esto es un mensaje");

La palabra **static** indica que lo que queremos ejecutar es una aplicación.
El comando **print** sólo imprime por consola. 
En el caso de **prinln** también dará un salto de línea al finalizar. 
Para imprimir un mensaje **por pantalla**, se utiliza el comando **JOptionPane.showMesaggeDialog(null,mensaje)**

Un comando similar al **prompt** de Javascript, es el siguiente:
Primero declaramos el tipo y la variable, luego el comando:
 
 	    String nombre=JOptionPane.showInputDialog("Ingrese su nombre");

En el caso de los tipos de dato numéricos, se debe agregar los comandos **Integer** y **parseInt**, previo a los demás comandos; por lo que quedaría así:

		int edad=Integer.parseInt(JOptionPane.showInputDialog("Ingrese su edad"));

		
Para imprimirlo por consola, el comando es:

	    System.out.println(nombre);

Y para imprimirlo por pantalla, el comando es:

        JOptionPane.showMessageDialog(null, "El nombre ingresado es "+ nombre); 

## TIPOS DE DATOS EN JAVA

Java es fuertemente tipado. Maneja los tipos de datos de manera muy estricta.
En Javascript no señalamos el tipo de dato acompañando a la variable. La variable toma el tipo de dato dependiendo del valor que le asignemos. 
En java debemos señalar el tipo de dato que vamos a almacenar. 

Existen 8 variables **primitivas** como son:

* byte (números enteros hasta 127)
* short
* int (generalmente para guardar números enteros se utiliza int)
* long 
* float (para almacenar números decimales)
* double (para decimales)
* char (para almacenar caracteres - 1 letra o 1 números)
* boolean (true o false)

Luego existen variables **de referencia** que serían los **objetos**, donde el tipo de dato representa una **clase**:  
* String (cadena de caracteres)

El String se diferencia de los otros, ya que inicia con mayúscula. Es del mismo tipo que la clase principal. 

