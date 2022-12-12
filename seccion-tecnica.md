# FUNDAMENTOS DE PROGRAMACION - ALGORITMOS JAVA Y JS


## LENGUAJE DE MÁQUINA 
Las instrucciones son cadenas binarias de 0 y 1.
* **Ventajas**: la máquina procesa las instrucciones de manera más rápida, por lo que implica una velocidad de ejecución superior a cualquier otro lenguaje.
* **Desventajas**: los programas sólo se pueden ejecutar en el mismo procesaodr, codificación más compleja y demorada, mayor incertidumbre (si nos equivocamos podemos dañar la máquina, al no haber un puente entre ambos).


## LENGUAJE DE BAJO NIVEL 
Por excelencia el lenguaje es Ensamblador o Assembler.
Son más fáciles de utilizar, pero también dependen de la máquina en particular (Difieren su arquitectura si se trabaja en Windows, en Linux, en MacOS, etc.).
Las instrucciones en Assembler son nemotécnicos, como por ejemplo las de operaciones aritméticas son ADD (SUM), SUB (RES), DIV, etc.
Estos lenguajes de bajo nivel requieren de una traducción al lenguaje máquina, para ser ejecutados por la computadora.
* **Ventajas**: mayor velocidad de codificación y de cálculo.
* **Desventajas**: dependencia de la máquina (programar en Windows es diferente que programar en Linux), y requiere de conocimientos de hardware de la máquina (un mal trabajo de programación puede traer problemas al hardware).


## LENGUAJE DE ALTO NIVEL 
Intentan mejorar los lenguajes de programación, la interpretación y el desarrollo.
Son los más utilizados por los programadores. Diseñados para que las personas escriban y entiendan los programas de una manera más fácil que los lenguajes anteriores.
Nos permiten controlar el acceso a secciones del sistema, y evitar posibles daños a la máquina.
* **Ventajas**: 
Independencia de la máquina. 
Pueden ejecutarse en diferentes tipos de computadoras.
Menor tiempo de aprendizaje. Reducción de costos. Se cuenta con procesos o funciones definidos previamente.
Un ejemplo es *Java*, ya que es multiplataforma, lo que se desarrolla se puede ejecutar en cualquier sistema.
* **Desventajas**:
No se aprovecha el 100% de los recursos de la máquina.
Se utiliza mayor memoria y el tiempo de ejecución es un poco mayor.

# FUNDAMENTOS DE ALGORITMIA

## Algoritmo

### Concepto
Es una secuencia lógica de pasos, para poder resolver un problema.
* *Precisos*: Deben tener un proceso lógico y específico.
* *Definidos*: Su comportamiento debe ser constante, siempre igual. Su resultado debe ser el mismo si lo ejecuto varias veces.
* *Finitos*: Debe ser una secuencia de pasos determinada, por lo que debe tener un fin.

### Cómo se componen
De tres partes.
* Entrada: los datos que recibe,
* Proceso: las acciones que se realizan sobre los datos de entrada,
* Salida: el resultado de las acciones sobre aquellos datos.

### Dos tipos de Algoritmos
* De la vida diaria:
Nos ayudan a resolver problemas cotidianos, que los realizamos de manera inconsciente. 
**Se puede dar solución a un problema de múltiples formas**
El algoritmo siempre debe tener un orden lógico.

* Computacional:
Permiten definir procesos para dar soluciones a distintos problemas, a través de operaciones lógicas en una máquina.
A diferencia del tipo anterior, se deben desarrollar siguiendo una metodología ya definida para la solución de problemas (como por ejemplo los lenguajes, sus sintaxis, etc.).

### Lenguajes Algorítmicos
Definen la manera en cómo nos comuniquemos mediante algoritmos, con el fin de que la máquina nos entienda.
Para resolver algoritmos, existen 4 técnicas diferentes para describir los pasos de un algoritmo de una manera más detallada y estructurada.
#### **LENGUAJE NATURAL**
Se utiliza un vocabulario cotidiano, para describir los problemas de una manera más simple.
#### **LENGUAJE DE DIAGRAMA DE FLUJO**
Algoritmos representados mediante símbolos, que facilitan el entendimiento de la solución.
Al ser un proceso gráfico, ayuda más a entender y realizar un seguimiento a la problemática.
#### **LENGUAJE DE PSEUDOCODIGO**
Cumplen la misma función que los diagramas de flujo, pero son orientados a definir la solución de un problema de una manera más precisa (ya no con gráficos), buscando definiciones formales.
Son más estructurados y definidos.
Son utilizados para crear fórmulas o atacar problemas mediante algoritmos computacionales.

* Características del Pseudocódigo:
- Debe ser preciso y definido (no pueden ser infinitos)
- Evitar múltiples interpretaciones (no ser ambiguos)
- Utilizar términos formales, pero relacionados al sentido común
- Eliminar instrucciones innecesarias

Cada lenguaje de programación define cómo se termina una línea de código (o sentencia), que generalmente es con un " **;** ".
Algunos lenguajes lo requieren (Java, Javascript, C#), otros no (Python).
Todos los algoritmos de pseudocódigo los finalizaremos con ese caracter de cierre.

*Reglas básicas del Pseudocódigo:
- Se debe delimitar entre un INICIO y FINAL
- Toda la lógica debe estar entre INICIO y FINAL
- Las variables que utilicemos en el algoritmo deben haber sido declaradas previamente
- Indicar el tipo de dato al que pertenece cada variable (en la mayoría de lenguajes)

#### **LENGUAJE DE PROGRAMACION**

