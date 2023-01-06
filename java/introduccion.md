# JAVA

- Es un lenguaje de programación orientado a objetos (POO).  
Todo lo que se trabaja en el lenguaje se debe pensar como objetos.
- Independiente de la Plataforma (Multiplataforma)  
Se puede trabajar desde windows, mac, linux, etc.
- Es un Lenguaje Interpretado   
El intérprete convierte el código java a código de máquina (JVM - Java Virtual Machine)

### **TECNOLOGIAS JAVA**

**JME (JAVA MICRO EDITION)**   
Aplicaciones móviles.  
**JSE (JAVA STANDARD EDITION)**    
Aplicaciones de escritorio (stand alone), applets, etc.  
**JEE (JAVA ENTERPRISE EDITION)**  
Aplicaciones empresariales (web), entorno cliente-servidor, software distribuido,etc. 

**JDK (JAVA DEVELOPMENT KIT)**
Es el software requerido para la creación de programas Java.  
Consiste en un conjunto de librerías y herramientas de desarrollo necesarias para los procesos de compilación y ejecución de las aplicaciones. 
Este a su vez trae dentro JRE.
Con JDK programo y ejecuto. 
Pero si vamos a instalar el software de un cliente, solo JRE que permite ejecutar.

**JRE (JAVA RUNTIME ENVIRONMENT)**
Es el entorno mínimo para la ejecución de programas. Sin estas, las aplicaciones Java no podrían ser ejecutadas satisfactoriamente. 

**ENTORNO DE DESARROLLO (IDE)**
Luego del proceso de instalación, podemos trabajar con Java desde diversos editores de texto almacenando el archivo con la extensión **.java**. 
Sin embargo, se debe usar un IDE para sacarle más provecho al lenguaje.  

- ECLIPSE
- NETBEANS
- INTELLIJ IDEA
- ORACLE JDEVELOPER 

### ESTRUCTURA DE UNA CLASE

Una clase equivale al archivo que contiene el código fuente de nuestro sistema. 
Un proyecto Java se puede componer de 1 o más clases. 
Deben tener un nombre igual al del archivo. 

### CONVENCIONES CLASES E INTERFACES

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

### PAQUETES

Por convención, llevan todo el nombre en minúsculas. 
Para utilizarlos, deben estar precedidos por la palabra **package**

*package paquete*;

Para poder utilizar los paquetes, las clases deben estar guardadas dentro de aquellos. 

### METODOS

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