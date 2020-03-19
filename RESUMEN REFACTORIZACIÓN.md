**REFACTORIZACIÓN**

1. **¿Qué es la refactorización?**
    
  Colección de técnicas individuales que sirven para mejorar el código existente.
La refactorización no es buscar errores ya que el código tiene que ser funcional, no es mejorar su rendimiento, ya que incluso puede funcionar mas lento y no es añadir nuevas características.
    
2. **Por qué y cuándo usar refactorización**

     Refactorizar facilita el desarrollo futuro, es decir, nos ayuda a ampliar el código más adelante.
     Para aquellos programas sirve refactorizar. Sin embargo si es una aplicación que es funcional y no va a ser ampliada, ni va a ser mantenida no hace falta refactorizar.

3. **El código con mal aspecto para la refactorización**

     Cuando en un código tenemos código repetido, métodos largos o con muchos comentarios se dice que ese código tiene mal aspecto, entonces nos vendría bien refactorizar.

4. **Pruebas automatizadas en la refactorización.**

     Cuando cambiamos el código podemos generar errores así que la mejor manera de tener el control del buen funcionamiento del código es hacer pruebas unitarias automáticas, ejecutándolas antes y después de refactorizar (JUnit en Java).

5. **La refactorización de extracción de método**

6. Las técnicas de refactorización se pueden agrupar en categorías:

   - **Nivel de método**
       para cuando queramos revisar si el nombre del método es correcto, si los
       parámetros tienen sentido, si hay demasiadas variables temporales o si hay
       código duplicado.

   - **Nivel de clase**
       para cuando queramos revisar si el método debe estar en la misma clase o si hay
       muchos métodos similares.

   - **Nivel de comunicación entre clases**
       para cuando queramos revisar si una clase está usando métodos de otra clase y
       por qué.

       

       **Extraer método:** Consiste en ver algo de código cuya lógica indique que se puedan crear un nuevo
       método a partir de esas líneas. Para hacer esto, movemos el código a un método
       nuevo. La cosa es tener muchos métodos con poco código.

7. **Método extractor de parámetros y variables**

     Esta técnica nos sirve para simplificar código con objetos y variables metiéndolos dentro de un método. Para el que tiene objetos tenemos que pasarle el objeto como parámetro y el de la variable metemos la variable y la porción de código dentro

8. **Usando el IDE en el método extractor para la refactorización**

     En los IDE hay un menú donde se pueden hacer refactorizaciones. En el caso de la extracción de un método, pulsamos en "Extract Method" tras haber seleccionado la porción del código y de esta forma hará el método automáticamente.

9. **Método de refactorización en línea**

     Buscamos una llamada a un método que no agregue ningún valor y lo fusionaremos con el método original.

10. **Refactorización que quita temporales**

     Se basa en minimizar el uso de variables temporales, por que estas nos pueden generar errores y aumenta la posibilidad de escribir métodos mas largos. Para ello convertimos la variable en una constante y creamos un método con la sentencia de la variable. Habrá que crear la llamada al nuevo método.
     Esta técnica es mas ineficiente pero mejora la legibilidad.

11. **Refactorización que añade temporales**

      Esta técnica se puede aplicar cuando queramos conseguir legibilidad en el código. Para ello podemos separar el código en distintas variables temporales.

12. **Refactorización moviendo métodos**

      Sirve para separar el método de una clase metiéndolo en otra clase. Así evitamos tener métodos que no son útiles en esa clase y así poder tener menos código.

13. **Refactorización de extraer métodos**

      Esta técnica sirve para extraer los elementos de una clase en la que no son necesarios metiéndolos en otra clase. Igual que en el anterior, esto sirve para tener menos código en una misma clase.

14. **Haciendo las condiciones mas fáciles de leer**

      Sirve para hacer mas legible las condiciones separándolas en métodos, los cuales mas adelante se podrán llamar.

15. **Refactorización de mover campos**

      Se basa en mover los datos de una clase a otra, en vez de mover los métodos. De esta manera simplifica mas cada clase.

16. **Trabajando con cúmulos de datos**

      En un código con un cumulo de datos que no estén atados a otros métodos podemos extraerlos en su propia clase.

17. **Simplificando llamadas al método y de los parámetros**

      Podemos hacer esto:

      - Renombrando métodos
      - Añadiendo o quitando parámetros

18. **Subir y bajar métodos y campos**

      Se basa en tomar el método o el campo y lo subimos de una subclase a la clase superior.

19. **Refinando jerarquías de clases**

      Tomamos los elementos iguales de una o varias clases y las ponemos en una nueva clase, la cual será una superclase de las demás.

20. **Refactorización a gran escala**

      Lo que hace esto es convertir diseños procedurales en objetos. 

