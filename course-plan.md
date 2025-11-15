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
  1. Abre [OnlineGDB](https://www.onlinegdb.com/) y crea un nuevo proyecto en **Java**.  
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
  Esta lección es fundamental para dotar al programa de inteligencia y la capacidad de repetir tareas, utilizando los conceptos de programación estructurada. Se inicia explicando 
  los Operadores, tanto Aritméticos (como el Módulo ``%``) como los Lógicos/de Comparación (``>``, ``==``), que son la base para crear las condiciones que el programa debe evaluar. Luego, se 
  introduce la estructura ``if-else`` para que el programa pueda tomar Decisiones, siguiendo un camino si una condición es Verdadera y otro si es Falsa. Finalmente, se explican los Bucles: 
  el bucle ``for`` (para repeticiones con un número fijo de vueltas) y el bucle ``while`` (para repeticiones que se mantienen mientras una condición sea Verdadera). El enfoque es simple: mostrar 
  cómo el programa "piensa" y cómo se evita escribir código repetitivo.


* **Enlace:** [Ver la lección](https://www.youtube.com/watch?v=8qf55AN8XU8)
* **Conclusiones clave:**
  
  - Los Operadores Aritméticos realizan cálculos; los Operadores Lógicos (``>``, ``==``) formulan preguntas de Verdadero/Falso.

  - La estructura ``if-else`` permite al código tomar decisiones y seguir rutas lógicas.

  - El bucle ``for`` se usa para repetir acciones un número de veces conocido.

  - El bucle ``while`` se usa para repetir acciones mientras una condición específica se cumpla.

  - Las estructuras de control son la base de la lógica para que un programa sea dinámico.

* **Práctica:** 

  1. Abre [JDoodle](https://www.jdoodle.com/online-java-compiler) y crea un nuevo proyecto en Java. Copia y ejecuta el siguiente código:
  
        ```java
        public class MyCode {
            public static void main(String[] args) {
                int hora = 14;
                int bateria = 3;
                      
                if (hora < 12) {
                    System.out.println("¡Buenos días!");
                } else {
                    System.out.println("¡Buenas tardes!");
                }
                    
                System.out.println("--- Alarma ---");
                for (int i = 0; i < 3; i++) {
                    System.out.println("Repetición: " + (i + 1));
                }
        
                while (bateria > 0) {
                    System.out.println("Batería: " + bateria + "%");
                    bateria = bateria - 1; 
                }
            }
        }
        ```
  2. Cambia el valor de ``hora`` a 9 y observa cómo cambia el resultado del ``if-else``.
  3. Cambia el número de repeticiones en el ``for`` (por ejemplo, ``i < 5``).

---
💡 *En la siguiente lección, aprenderás a usar Métodos para que tu código sea aún más limpio y organizado, utilizando funciones reutilizables.*

### **Lección 4:** Métodos y parametros

* **Descripción:**
  Esta lección introduce la noción de modularidad en la programación, explicando cómo los Métodos (o funciones) permiten agrupar bloques de código
  para realizar una tarea específica. Esta es una excelente práctica para la reutilización del código. Se define qué son los Parámetros (datos de 
  entrada) y cómo se usan para hacer que un método sea flexible (por ejemplo, el método ``saludar`` funciona para cualquier nombre que se le pase). 
  Finalmente, se explica el concepto de Retorno, demostrando cómo un método puede calcular un valor y entregárselo de vuelta al programa principal.
  Los ejemplos se enfocan en la creación de funciones reutilizables que simplifican el código principal.

* **Enlace:** [Ver la lección](https://www.youtube.com/watch?v=nPyWHS-9HqM&t=12s)
* **Conclusiones clave:**

  - Un Método es un bloque de código reutilizable que ayuda a mantener el programa organizado.

  - Los Parámetros son los datos que el método necesita para funcionar y van entre paréntesis.

  - ``void`` significa que el método solo ejecuta acciones, pero no devuelve un valor.

  - El Retorno (usando la palabra ``return``) permite que un método entregue un resultado calculado al resto del programa, creando una función reutilizable.

  - Los métodos son la base para construir las Clases y Objetos en POO.
* **Práctica:** 

  1. Abre [JDoodle](https://www.jdoodle.com/online-java-compiler) y crea un nuevo proyecto en Java. Copia y ejecuta el siguiente código:

        ```java
        public class MyCode {

            public static void imprimir(String texto) {
                System.out.println("--- " + texto + " ---");
            }

            public static int sumarDiez(int numero) {
                int resultado = numero + 10;
                return resultado;
            }

            public static void main(String[] args) {
                imprimir("INICIO DEL PROGRAMA");

                int miNumero = 5;
                int total = sumarDiez(miNumero);
        
                System.out.println("5 + 10 es: " + total); 
        
                imprimir("FIN DEL PROGRAMA");
            }
        }
        ```
    2. Cambia el número ``5`` en ``sumarDiez(5)`` a otro valor y observa cómo cambia la variable ``total``.     
    3. Intenta llamar al método ``imprimir()`` con un texto diferente.

 ---
💡 *La siguiente lección nos llevará a la Programación Orientada a Objetos, donde usaremos los métodos para dar comportamiento a las Clases y Objetos.*

## Módulo 3: Introducción a Programación Orientada a Objetos (POO)

### **Lección 5:** Clases, objetos y constructores

* **Descripción:**
  Introducción a la Programación Orientada a Objetos (POO) en Java, explicando qué son las clases y los objetos usando ejemplos del mundo real. Se crea una clase simple Estudiante con atributos, constructor y un método.  
* **Enlace:** [Ver la lección](https://youtu.be/-gOkco98jZU)  
* **Conclusiones clave:**  
  * Una clase es una plantilla o molde que describe las características y comportamientos de algo (por ejemplo, un estudiante).  
  * Un objeto es una instancia de una clase: cada objeto tiene sus propios valores para los atributos.  
  * Un constructor es un método especial que se usa para crear objetos e inicializar sus atributos.  
  * Los métodos permiten que los objetos realicen acciones (como presentarse).  
* **Práctica:** 
Abre [OnlineGDB](https://www.onlinegdb.com/) y selecciona en la parte de la derecha el lenguaje Java, luego crea un nuevo archivo llamado Estudiante.Java y coloca el siguiente código  
 ```Java
// Clase Estudiante
public class Estudiante {
    String nombre;
    int edad;
    double promedio;

    // Constructor
    Estudiante(String n, int e, double p) {
        nombre = n;
        edad = e;
        promedio = p;
    }

    // Método
    void presentarse() {
        System.out.println("Hola, soy " + nombre + ", tengo " + edad + " años.");
        System.out.println("Mi promedio es: " + promedio);
    }
}

```
 Luego en la clase Main, coloca lo siguiente  

 ```Java
 // Clase Main para probar Estudiante
public class Main {
    public static void main(String[] args) {
        Estudiante estudiante1 = new Estudiante("Ana", 15, 17.5);
        Estudiante estudiante2 = new Estudiante("Luis", 16, 18.2);

        estudiante1.presentarse();
        estudiante2.presentarse();
    }
}

 ```

### **Lección 6:** Encapsulación y métodos (``getters`` y ``setters``)

* **Descripción:** Se introduce el concepto de encapsulación para proteger los datos de una clase. Se modifican los atributos de Estudiante a private y se añaden métodos getters y setters para acceder y modificar los datos de forma controlada.
* **Enlace:** [Ver la lección](https://youtu.be/BYYhNhY-Lbg)
* **Conclusiones clave:**  
  * La encapsulación consiste en proteger los datos de una clase, evitando que se modifiquen directamente desde fuera.

  * La palabra clave private hace que un atributo solo pueda ser accedido dentro de la misma clase.

  * Los getters permiten leer el valor de un atributo de manera segura.

  * Los setters permiten cambiar el valor de un atributo, aplicando validaciones si es necesario (por ejemplo, no permitir edades negativas).

  * Encapsular mejora la seguridad y la organización del código, especialmente en proyectos grandes.
* **Práctica:** 
En la clase Estudiante, actualiza con el siguiente código
 ```Java
// Clase Estudiante con encapsulación
public class Estudiante {
    private String nombre;
    private int edad;
    private double promedio;

    // Constructor
    Estudiante(String n, int e, double p) {
        nombre = n;
        edad = e;
        promedio = p;
    }

    // Getters
    public String getNombre() {
        return nombre;
    }

    public int getEdad() {
        return edad;
    }

    public double getPromedio() {
        return promedio;
    }

    // Setters
    public void setNombre(String nuevoNombre) {
        nombre = nuevoNombre;
    }

    public void setEdad(int nuevaEdad) {
        if (nuevaEdad >= 0) {
            edad = nuevaEdad;
        }
    }

    public void setPromedio(double nuevoPromedio) {
        if (nuevoPromedio >= 0 && nuevoPromedio <= 20) {
            promedio = nuevoPromedio;
        }
    }

    // (Opcional) Método de presentación
    public void presentarse() {
        System.out.println("Hola, soy " + nombre + ", tengo " + edad + " años.");
        System.out.println("Mi promedio es: " + promedio);
    }
}


 ```
Ahora actualiza la clase Main  
```Java
// Clase Main para probar getters y setters
public class Main {
    public static void main(String[] args) {
        Estudiante estudiante = new Estudiante("Ana", 15, 17.5);

        // Modificar datos usando setters
        estudiante.setEdad(16);
        estudiante.setPromedio(18.0);

        // Leer datos usando getters
        System.out.println("Nombre: " + estudiante.getNombre());
        System.out.println("Edad: " + estudiante.getEdad());
        System.out.println("Promedio: " + estudiante.getPromedio());

        // (Opcional) llamar al método presentarse
        estudiante.presentarse();
    }
}

```


## Módulo 4: Proyecto Final

### **Lección 7:** Programa final (mini proyecto en Java)

**Descripción:** En esta lección, los estudiantes desarrollarán un proyecto completo en Java, aplicando los conceptos vistos en todo el curso: clases, objetos, métodos, getters/setters y lectura de datos.
  El mini proyecto se titula “Registro de Estudiantes”, donde podrán:

  * Agregar estudiantes
  * Listar estudiantes
  * Buscar estudiantes por nombre

Este ejercicio les permite crear un programa real usando Programación Orientada a Objetos.

**Enlace:** [Ver la lección](https://youtu.be/YSCQAqwQtk8)

**Conclusiones clave:**

  * Un proyecto real en Java combina varias clases que trabajan juntas.
  * La POO organiza mejor el código y permite representar cosas del mundo real.
  * Una lista (`ArrayList`) permite almacenar múltiples objetos.
  * La interacción por consola permite al usuario navegar por un menú sencillo.
  * Aplicar todo lo aprendido refuerza el entendimiento de Java como lenguaje.

**Práctica: Mini proyecto “Registro de Estudiantes”** 

1. Crea dos archivos en Replit:

    - `Estudiante.java`
    
    - `Main.java`
    - 
2. Copia el siguiente código en cada archivo:

**Estudiante.java**

```Java
public class Estudiante {
    private String nombre;
    private int edad;
    private double promedio;

    public Estudiante(String nombre, int edad, double promedio) {
        this.nombre = nombre;
        this.edad = edad;
        this.promedio = promedio;
    }

    public String getNombre() {
        return nombre;
    }

    public void mostrarInfo() {
        System.out.println("Nombre: " + nombre);
        System.out.println("Edad: " + edad);
        System.out.println("Promedio: " + promedio);
        System.out.println("------------------------------");
    }
}

````

**Main.java**

```Java
import java.util.ArrayList;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        ArrayList<Estudiante> lista = new ArrayList<>();

        int opcion = 0;

        while (opcion != 4) {
            System.out.println("\n=== REGISTRO DE ESTUDIANTES ===");
            System.out.println("1. Agregar estudiante");
            System.out.println("2. Mostrar todos");
            System.out.println("3. Buscar por nombre");
            System.out.println("4. Salir");
            System.out.print("Elige una opción: ");
            opcion = input.nextInt();
            input.nextLine();  

            if (opcion == 1) {
                System.out.print("Nombre: ");
                String nombre = input.nextLine();

                System.out.print("Edad: ");
                int edad = input.nextInt();

                System.out.print("Promedio: ");
                double prom = input.nextDouble();
                input.nextLine();

                Estudiante e = new Estudiante(nombre, edad, prom);
                lista.add(e);

                System.out.println("Estudiante agregado correctamente!");

            } else if (opcion == 2) {
                if (lista.isEmpty()) {
                    System.out.println("No hay estudiantes registrados.");
                } else {
                    for (Estudiante e : lista) {
                        e.mostrarInfo();
                    }
                }

            } else if (opcion == 3) {
                System.out.print("Ingresa el nombre a buscar: ");
                String buscar = input.nextLine();

                boolean encontrado = false;

                for (Estudiante e : lista) {
                    if (e.getNombre().equalsIgnoreCase(buscar)) {
                        e.mostrarInfo();
                        encontrado = true;
                    }
                }

                if (!encontrado) {
                    System.out.println("No se encontró ese nombre.");
                }
            }
        }

        System.out.println("¡Fin del programa!");
    }
}

````
### **Lección 8:** Mejores prácticas y próximos pasos

**Descripción:** Esta última lección brinda consejos esenciales para escribir código más limpio y profesional, además de motivar a los estudiantes a seguir aprendiendo programación.
  Se mencionan errores comunes, cómo depurarlos, y sugerencias para continuar practicando Java.

**Enlace:** [Ver la lección](https://youtu.be/pUdu7chmEds)

**Conclusiones clave:**

* Escribir código limpio facilita entender y mantener los programas.
* Divide tu lógica en métodos y clases para evitar repetir código.
* Usa nombres claros y significativos para variables y funciones.
* Comenta partes importantes del código.
* Equivocarte es parte fundamental de aprender a programar.
* Los proyectos pequeños son la mejor forma de mejorar habilidades.

**Práctica:** Los estudiantes deberán:

1. Revisar su proyecto final e implementar 3 mejoras, como:

* Agregar getters y setters.
* Validar datos (ej. evitar promedios negativos o mayores a 20).
* Crear un nuevo método (por ejemplo, determinar si el estudiante está aprobado).
* Añadir una opción al menú (ej. eliminar estudiante o editar datos).

2. Subir su versión final a Replit.

3. Reflexionar brevemente por escrito:

* ¿Qué fue lo más difícil?
* ¿Qué fue lo que más te gustó de crear tu primer proyecto en Java?

## Recursos Adicionales

| Nº de Lección | Actividad                           | Enlace                                                                       |
|---------------|-------------------------------------|------------------------------------------------------------------------------|
| 1             | ¿Qué es Java y la Programación?     | [Abrir OnlineGDB Hola Mundo](https://www.onlinegdb.com/)                     |
| 2             | Variables y Tipos de Datos          | [Abrir OnlineGDB Scanner](https://www.onlinegdb.com/)                        |
| 3             | Operadores y extructuras de control | [Abrir JDoodle Estructuras](https://www.jdoodle.com/online-java-compiler)    | 
| 4             | Métodos y parametros                | [Abrir JDoodle Funciones](https://www.jdoodle.com/online-java-compiler)      |
| 5             | Clases, objetos y constructores     | [Abrir OnlineGDB Introducción a POO](https://onlinegdb.com/cfCbsQJ3Yw)       |
| 6             | Encapsulación y métodos             | [Abrir OnlineGDB Encapsulación](https://onlinegdb.com/amlAnJeRdz)            |
| 7             | Programa final                      | [Abrir JDoodle Proyecto Final](https://www.jdoodle.com/online-java-compiler) |


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
