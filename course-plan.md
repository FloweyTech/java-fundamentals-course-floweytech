# Fundamentos de Java para Principiantes

## Resumen del Curso

Este curso de aproximadamente una hora de duración fue diseñado por **FloweyTech** para introducir a estudiantes de secundaria al fascinante mundo de la programación con Java.
A través de ejemplos claros, visuales y cercanos a su día a día, los participantes aprenderán paso a paso los principios esenciales de la **Programación Orientada a Objetos (POO)** y cómo aplicarlos en programas reales.

El aprendizaje se construye mediante lecciones breves y progresivas, combinando teoría sencilla con práctica inmediata en plataformas online.
El objetivo es que los estudiantes entiendan cómo “piensa” un programador y adquieran las bases necesarias para continuar su formación en el desarrollo de software.

## Objetivo del Curso

Al finalizar el curso, el estudiante será capaz de:

* Comprender los conceptos básicos de la programación estructurada y orientada a objetos.
* Crear programas simples en Java utilizando variables, estructuras de control y métodos.
* Modelar pequeños problemas del mundo real mediante clases y objetos.
* Reconocer la importancia de las buenas prácticas al escribir código.

El enfoque de FloweyTech es aprender haciendo: cada tema teórico se acompaña de un ejercicio guiado que puede ejecutarse y modificarse directamente en el navegador.

## Público Objetivo

El curso está dirigido a estudiantes de 12 a 17 años, curiosos por la tecnología y sin experiencia previa en programación.
El lenguaje usado es sencillo, los ejemplos son cercanos (basados en situaciones cotidianas), y se evita el uso de tecnicismos innecesarios para mantener el proceso de aprendizaje ameno y accesible.

## Prerrequisitos

No se requiere ningún conocimiento previo de programación ni instalación de software.
Solo se necesita una computadora con conexión a internet y ganas de experimentar con código.

## Herramientas Necesarias

Todo el contenido se desarrolla en entornos 100 % online y gratuitos, accesibles desde cualquier navegador moderno (Chrome, Firefox, Edge o Safari).
Durante el curso se utilizan los siguientes editores de código en línea:

* [Replit](https://replit.com/) → para practicar ejemplos interactivos.
* [JDoodle](https://www.jdoodle.com/) → para ejecutar fragmentos de código breves.
* [OnlineGDB](https://www.onlinegdb.com/) → para visualizar proyectos orientados a objetos.

Los estudiantes pueden probar, modificar y ejecutar código sin instalar nada en su computadora, lo que permite un aprendizaje ágil y libre de barreras técnicas.

## Repositorio de Código Fuente
El código fuente completo del curso está disponible en el siguiente repositorio de GitHub:
* [Repositorio de Fundamentos de Java para Principiantes](https://github.com/FloweyTech/java-fundamentals-course-floweytech.git)

## Módulo 1: Introducción y fundamentos básicos

### **Lección 1:** ¿Qué es Java y la Programación?

* **Descripción:**  
  En esta primera lección, los estudiantes conocerán qué significa programar y cómo Java permite convertir ideas en instrucciones que una computadora puede entender.  
  A través de ejemplos sencillos y comparaciones cotidianas, se explica que programar es dar pasos ordenados para resolver un problema, y que Java es un lenguaje versátil usado en millones de dispositivos: desde celulares Android hasta sistemas bancarios o videojuegos.  
  Se muestra el clásico ejemplo “Hola Mundo” como el primer vistazo al código, explicando de forma simple cómo el programa sigue las instrucciones dentro del método principal.  
  Finalmente, se presenta una pequeña demostración en la que Java realiza una suma básica, anticipando los conceptos que se desarrollarán en la siguiente lección sobre variables y tipos de datos.

* **Enlace:** [Ver la lección](https://youtu.be/JMmJFuvtKEA)

* **Conclusiones clave:**  
  - Programar es dar instrucciones paso a paso a una computadora.  
  - Java es un lenguaje multiplataforma, estable y muy usado en el mundo real.  
  - Todo programa en Java comienza dentro de una estructura llamada `main`.  
  - Con una sola línea, Java puede mostrar mensajes y realizar operaciones simples.  
  - En la siguiente lección se aprenderá a guardar información en **variables** para hacer programas más dinámicos.

* **Práctica:**  
  1. Abre [OnlineGDB]([https://replit.com/~](https://www.onlinegdb.com/)) y crea un nuevo proyecto en **Java**.  
  2. Copia este código y ejecútalo:
     ```java
     public class Main {
         public static void main(String[] args) {
             System.out.println("Hola mundo desde FloweyTech!");
             System.out.println(5 + 3);
         }
     }
     ```
  3. Cambia los números de la suma o el texto del mensaje para ver cómo el resultado cambia.  
  4. Observa que todo lo que está dentro de las llaves `{ }` se ejecuta al iniciar el programa.  
  5. Guarda tu proyecto: este será el punto de partida para la **Lección 2: Variables y tipos de datos**.


### **Lección 2:** Variables y Tipos de Datos

* **Descripción:**  
  En esta segunda lección, los estudiantes aprenden qué son las **variables** y los **tipos de datos** en Java, conceptos fundamentales para crear programas dinámicos.  
  A través de ejemplos visuales, se explica que una variable es como una **caja con nombre** donde se guarda información que puede cambiar durante la ejecución del programa.  
  Se presentan los tipos de datos más comunes —**int**, **double**, **String** y **boolean**— junto con ejemplos sencillos que muestran cómo almacenar números, texto y valores verdaderos o falsos.  
  Finalmente, se desarrolla un pequeño programa que solicita datos al usuario (nombre, edad y número de compañeros), realiza una **suma** y muestra un mensaje personalizado con el resultado.

* **Enlace:** [Ver la lección](https://youtu.be/YulS5Sox-3c)

* **Conclusiones clave:**  
  - Una variable es un espacio de memoria donde el programa guarda información.  
  - Cada variable tiene un **nombre** y un **tipo de dato**.  
  - Los tipos básicos más usados son:  
    - `int` → números enteros.  
    - `double` → números con decimales.  
    - `String` → texto o palabras.  
    - `boolean` → valores de verdadero o falso.  
  - Las variables permiten que los programas **recuerden, calculen y combinen información**.  
  - Con el objeto **Scanner** podemos pedir datos al usuario e interactuar con ellos.  

* **Práctica:**  
  1. Crea un nuevo proyecto en [GDB](https://www.onlinegdb.com/) usando **Java**.  
  2. Copia el siguiente código y ejecútalo:
     ```java
     import java.util.Scanner;  // Permite leer datos del teclado

     public class Main {
         public static void main(String[] args) {
             Scanner input = new Scanner(System.in); // Crea el lector de entrada

             System.out.println("¿Cuál es tu nombre?");
             String nombre = input.nextLine();

             System.out.println("¿Cuántos años tienes?");
             int edad = input.nextInt();

             System.out.println("¿Cuántos compañeros varones hay en tu salón?");
             int varones = input.nextInt();

             System.out.println("¿Cuántas compañeras mujeres hay?");
             int mujeres = input.nextInt();

             int total = varones + mujeres; // Calcula el total de compañeros

             System.out.println("\n----------------------------");
             System.out.println(nombre + " tiene " + edad + " años y " + total + " compañeros de clase.");
             System.out.println("----------------------------");
         }
     }
     ```
  3. Ejecuta el programa y responde a las preguntas en consola.  
  4. Observa cómo el programa **usa tus respuestas** para generar el mensaje final.  
  5. Cambia los nombres de las variables o los textos para experimentar.  

---

💡 *En la siguiente lección, aprenderás cómo usar estructuras de control como `if`, `else`, `for` y `while` para que tu programa pueda tomar decisiones y repetir acciones.*


## Módulo 2: Lógica y control de flujo

### **Lección 3:** Operadores y extructuras de control (``if``, ``else``, ``for``, ``while``)

* **Descripción:**
* **Enlace:** [Ver la lección]()
* **Conclusiones clave:**
* **Práctica:** 

### **Lección 4:** Métodos y parametros

* **Descripción:**
* **Enlace:** [Ver la lección]()
* **Conclusiones clave:**
* **Práctica:** 

## Módulo 3: Introducción a Programación Orientada a Objetos (POO)

### **Lección 5:** Clases, objetos y  constructores

* **Descripción:**
* **Enlace:** [Ver la lección]()
* **Conclusiones clave:**
* **Práctica:** 

### **Lección 6:** Encapsulación y métodos (``getters`` y ``setters``)

* **Descripción:**
* **Enlace:** [Ver la lección]()
* **Conclusiones clave:**
* **Práctica:** 

## Módulo 4: Proyecto Final

### **Lección 7:** Programa final (mini proyecto en Java)

* **Descripción:**
* **Enlace:** [Ver la lección]()
* **Conclusiones clave:**
* **Práctica:** 

### **Lección 8:** Mejores prácticas y próximos pasos

* **Descripción:**
* **Enlace:** [Ver la lección]()
* **Conclusiones clave:**
* **Práctica:** 

## Recursos Adicionales

| Nº de Lección | Actividad | Enlace |
| ------------- |-----------|--------|
| 1             |           |        |
| 2             |           |        |
| 3             |           |        |
| 4             |           |        |
| 5             |           |        |
| 6             |           |        |
| 7             |           |        |


## Elaboración

**Universidad Peruana de Ciencias Aplicadas (UPC)** <br>
**Carrera de Ingeniería de Software** <br>
**Período 202520**<br>
**1ASI0729 Desarrollo de Aplicaciones Open Source**<br>
NRC 7349 <br>
**Nombre del equipo**: FloweyTech <br>
**Líder del equipo**: Anjali Amaro Villar <br>
**Integrantes del equipo**: 
- Quique Vladimir Jara Benites
- Gonzalo Samuel Quintanilla Pozo
- Diego Alejandro Vilca Saboya <br>

**Fecha de entrega**: 15 de noviembre de 2025 
