# EJERCICIOS EN JAVA

## EJERCICIO 1
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

### **APLICACION . JAVA**
<br> 

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

## EJERCICIO 2
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

### **APLICACION . JAVA**
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
