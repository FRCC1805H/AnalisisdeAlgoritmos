# AnalisisdeAlgoritmos
## Fecha 14/04/2025
## Nombre Fabian Cañar

# Lib Fundamentos de Algoritmia 

# Resumen de los libros Capitulo 1 

# Preliminares 

## Introduccion 
En este libro hablaremos de algoritmos y de algoritmia. Este capítulo introductorio define en primer lugar lo que queremos decir con estas dos palabras. lustraremos esta discusión formal mostrando varias formas de realizar una sencilla multiplicación. También las tareas de todos los días poseen profundidades ocul-tas. Además aprovecharemos la oportunidad para explicar por qué pensamos que el estudio de los algoritmos es a la vez útil e interesante.

Aquellas personas que tengan olvidadas sus matemáticas básicas y sus ciencias de la computación, deberían cuando menos leer los principales resultados que presentamos para refrescar su memoria. Nuestra presentación es sucinta e informal y no pretende ocupar el puesto de cursos de análisis elemental, de cálculo ni de programación, La mayoría de los resultados que damos se necesitarán posteriormente en el libro; a la inversa, en los capítulos posteriores intentaremos no utilizar resultados que vayan más allá de las bases que se han reunido en este capítulo.

## ¿QUÉ ES UN ALGORITMO?
Un algoritmo, nombre que proviene del matemático persa del siglo IX al-Khowarizmi, es sencillamente un conjunto de reglas para efectuar algún cál-culo, bien sea a mano o, más frecuentemente, en una máquina. En este libro nos preocupan fundamentalmente los algoritmos que van a ser utilizados en una computadora. Sin embargo, también podrían incluirse otros métodos sistemáticos para calcular un resultado; los métodos que aprendimos en la escuela para sumar, multiplicar y dividir números, son también algoritmos, por ejemplo. Muchos monaguillos ingleses, aburridos por pláticas poco intere-santes, pasan el tiempo calculando la fecha de Pascua y empleando el algoritmo que se emplea en el Devocionario Anglicano. El algoritmo más famoso de la historia procede de un tiempo anterior al de los antiguos griegos: se trata del algoritmo de Euclides para calcular el máximo común divisor de dos enteros.

La ejecución de un algoritmo no debe de implicar, normalmente, ninguna decisión subjetiva, ni tampoco debe de hacer preciso el uso de la intuición ni de la creatividad. Por tanto se puede considerar que una receta de cocina es un algoritmo si describe precisamente la forma de preparar un cierto plato, proporcionándonos las cantidades exactas que deben de utilizarse y también instrucciones detalladas acerca del tiempo que debe de guisarse. Por otra parte, si se incluyen nociones vagas tales como «salpimentar a su gusto» o «guísese hasta que esté medio hecho» entonces no se podría llamar algoritmo.

Una instrucción tal como «seleccionar un número entre 1 y 6» si no se da ningún detalle más, no es admisible en un algoritmo. Sin embargo, sería aceptable decir «seleccionar un número entre 1 y 6 de tal manera que todos los valores tengan la misma probabilidad de ser seleccionados». En este caso, cuando se ejecute el algoritmo manualmente, quizá decidamos obedecer esta instrucción tirando un dado sin cargar; en una computadora, podríamos implementarlo utilizando un generador de números pseudoaleatorios.

![image](https://github.com/user-attachments/assets/ebde8c33-65ab-4bc6-bce7-2b42669d9102)

https://www.youtube.com/watch?v=U3CGMyjzlvM


## NOTACIÓN PARA LOS PROGRAMAS
Es importante decidir la forma en que vamos a describir nuestros algoritmos. Si intentamos explicarlos en español, descubriremos rápidamente que los lenguajes naturales no están en absoluto adaptados para este tipo de cosas. Para evitar la confusión, en el futuro especificaremos nuestros algoritmos dando el correspondiente programa. Suponemos que el lector está familiarizado con al menos un lenguaje de programación bien estructurado, tal como Pascal. Sin embargo, no nos limitaremos estrictamente a ningún lenguaje de programación concreto: de esta manera, los aspectos esenciales de un algoritmo no resultarán oscurecidos por detalles de programación relativamente poco importantes, y realmente no importa cuál sea el lenguaje bien estructurado que prefiera el lector.

Hay algunos aspectos de nuestra notación para los programas que merecen especial atención. Utilizaremos frases en español en nuestros programas siempre que esto produzca sencillez y claridad. De manera similar, utilizaremos el lenguaje matemático, tal como el del álgebra y de la teoría de conjuntos, siempre que sea necesario (incluyendo símbolos tales como - y L que se presentan en la Sección 1.4.7). Como consecuencia, una sola «instrucción» de nuestros programas puede tener que traducirse a varias instrucciones, quizá a un bucle mientras, si es que el algoritmo tiene que implementarse en un lenguaje de programación con vencional.

En los procedimientos y funciones no se declara el tipo de los parámetros, ni tampoco el tipo de los resultados proporcionados por una función, a no ser que tales declaraciones hagan que el algoritmo sea más fácil de entender. Los parámetros escalares se pasan por valor, lo que significa que son tratados como variables locales dentro del procedimiento o la función, a no ser que se decla-Ten como parámetros var, en cuyo caso se pueden utilizar para proporcionar un valor al programa llamante. En contraste, los parámetros tipo matriz se pasan por referencia, lo cual significa que toda modificación efectuada dentro del procedimiento o función se verán reflejados en la matriz que realmente se pase en la instrucción que haga la llamada.

Por último, supondremos que el lector está familiarizado con los conceptos de recursividad, registro y puntero. Estos dos últimos se denotan exactamente como en Pascal, salvo por la omisión de begin y end en los records. En par-ticular, los punteros se denotan con el símbolo «T».

## NOTACIÓN MATEMATICA
Esta sección revisa la notación matemática que utilizaremos a lo largo del libro.
Nuestra revisión es sucinta, por cuanto suponemos al lector familiarizado con la mayor parte de ella. Sin embargo, recomendamos leerla al menos de forma rápida porque presentamos la mayoría de los símbolos que se van a utilizar, y algunos de ellos (tales como [i.jl, V, 7, Ig, Lx], ÷ y R2) no gozan de aceptación universal.
### Cálculo proposicional
Existen dos «valores de verdad», verdadero y falso. Una variable booleana (o proposi-cional) solamente puede tomar uno de estos dos valores. Si p es una variable boo-leana, escribimos p es verdadero, o bien simplemente p, para indicar p - verdadero.
Esto es generalizable a todas las expresiones arbitrarias cuyo valor sea booleano.

Sean p y q dos variables booleanas. Su conjunción p ^q, o p y q es verdadero si y sólo si p y 9 son verdaderos. Su disyunción pv 4, 0 p o q es verdadero si y sólo si al menos uno de entre p o q es verdadero. (En particular, la disyunción de p y q es verdadera cuando tanto p como q son verdaderos.) La negación de p que se denota como -p o «no p», es verdadero si y sólo si p es falso. 

Si la verdad de p implica la de q escribiremos p →q, que se lee si p entonces q. Si la verdad de p es equivalente a la de q, lo cual significa que son ambos o bien verdadero o bien falso, entonces escribimos p → q. Podemos construir fórmulas booleanas a partir de variables boo-leanas, constantes (verdadero y falso), conectivas (n, v, -, →, →) y paréntesis de la forma evidente.
### Teoria de conjuntos

 Un conjunto se dice finito si contiene un número finito de elementos; en caso contrario el conjunto es infinito. Si X es un conjunto finito, IXI, la cardinalidad de X denota el número de elementos que hay en X. Si X es un conjunto infinito podemos escribir que la cardinalidad de X es infinita. El conjunto vacío, que se denota como o, es el conjunto único cuya cardinalidad es 0.
 
La forma más sencilla de denotar un conjunto es rodear la enumeración de esos elementos entre llaves. Por ejemplo, (2,3,5,7), denota el conjunto de números primos de una sola cifra. Cuando no puede surgir ninguna ambiguedad, se permite el uso de puntos suspensivos, tal como en «N= [0,1,2,3, ...] es el conjunto de números naturales».

Si X es un conjunto, x eX significa que x pertenece a X. Escribiremos que x e X cuando x no pertenezca a X. La barra vertical « |» se lee en la forma «tal que» y se utiliza para definir un conjunto describiendo la propiedad que cumplen todos sus miembros. Por ejemplo, in In e N y n es impar) denota el conjunto de todos los números naturales impares. Hay otras notaciones alternativas más sencillas para el mismo conjunto que son In e N In es impar) o incluso (2n + 1 | n € N).

Si X e Y son dos conjuntos, X = Y significa que todos los elemento de X pertenecen también a Y; y se lee «X es un subconjunto de Y», La notación X c Y significa que X ≤ Y y además que hay por lo menos un elemento de Y que no pertenece a X; se lee «X es un subconjunto propio de Y». Tenga en cuenta que algunos autores utilizan c para denotar lo que nosotros denotamos mediante s. 
Los conjuntos X e Y son iguales, lo cual se escribe X = Y, si y sólo si contienen exactamente los
mismos elementos. Esto es equivalente a decir que X = Y y que Y = X.

Si X e Y son dos conjuntos, denotamos su unión mediante X uY=|z |z € X oz e Y,su intersección como X nY - (z | z € X y z e Yl, y su diferencia como
X \Y = (z | ze X peroz e Y).

### Enteros, reales e intervalos
Es el proceso de evaluar el rendimiento de un algoritmo en términos de:
* Eficiencia temporal (tiempo de ejecución).
* Eficiencia espacial (uso de memoria).
* Corrección y estabilidad numérica si trabaja con números reales o intervalos
### Funciones y relaciones
Una función en este contexto representa cómo crece el tiempo de ejecución ( o uso(o uso de memoria) de un algoritmo en relación con el tamaño de la entrada) .( n)
Relación de recurrencia : Se utiliza en algoritmos recursivos para describir el tiempo de ejecución en función del tamaño del problema.
Ejemplo clásico:

T(n) = 2T(n/2) + n→ relación del algoritmo de MergeSort.

Relación entre entradas y salidas : Se analiza cómo una entrada específica se transforma en una salida y qué tan costoso es ese proceso.

Relación de orden : Permite clasificar algoritmos según su eficiencia.

Por ejemplo:
O(log n) ⊂ O(n) ⊂ O(n log n) ⊂ O(n²)
(orden creciente de complejidad)


# Resumen de los libros Capitulo 2 

# ALGORITMIA ELEMENTAL

## INTRODUCCIÓN
La algoritmia es eles el estudio, diseño y análisis de algoritmos , es decir, secuencias finitas de pasos bien definidos que permiten resolver un problema o realizaro realizar una tarea de forma sistemática.

Un algoritmo es como unaes como una receta o instrucción paso a paso para lograr un objetivo, ya sea en programación, matemáticas, lógica o la vida cotidiana.

## ERICIENCIA DE LOS ALGONITMOS
La eficiencia de un algoritmo se refiere ade un algoritmo se refiere a qué tan bien utilizar los recursos disponibles ( como el tiempo(como el tiempo de ejecución y la memoriay la memoria ) al resolver un problema.

Un algoritmo eficiente resuelve el problema correctamente usando la menor cantidad de recursos posible .

*Del tamaño de la entrada ( n)
*Del tipo de operaciones realizadas
*La estructura del algoritmo
*Del lenguaje y entorno de ejecución

Un algoritmo eficiente no solo funciona , sino que lo hace de forma óptima .
En programación real, elegir un algoritmo eficiente puede marcar la diferencia entre un programa utilizable y uno lento o inservible.

## ANÁLISIS DE (CASO MEDIOS) Y DE (CASO PEOR)
En el análisis de algoritmos, se estudia cómo se comporta un algoritmo según el tipo de entrada que recibe. Dos casos fundamentales son :que recibe. Dos casos fundamentales son:

### Caso Peor

Es la situación en la que el algoritmo tarda más tiempo posible en completarseen completarse, debido a una entrada desfavorable.
Ayuda a garantizar el límite máximo de tiempo o recursos que puedes usarque puede usar un algoritmo.
Se representa con la notación O (Big O) .

### Ejemplo

*En una búsqueda lineal de un elemento en una lista de nelementos:
*El caso peor ocurre cuando el elemento no está en la lista .
*Se revisan los nelementos → O(n) .

### Caso Medio 

Es el tiempo promedio que toma un algoritmo en una gran cantidad de ejecuciones, considerando todas las entradas posibles .
Da una estimación más realista del rendimiento del algoritmo en la práctica.
Se representa con la notación Θ (Theta).

### Ejemplo 

*Si el elemento está en una posición aleatoria.
*El caso medio es buscar después de recorrer la mitad de los elementos → Θ(n/2) , pero se simplifica como Θ(n) .

## ¿QUÉ ES LINA OPERACIÓN ELEMENTAL?

Una operación elemental es una acciónes una acción básica e indivisible queque realiza un algoritmo y que consume un tiempo constante , es decir, su tiempo de ejecución no depende del tamaño de la entrada .
Al analizar un algoritmo, se cuentan las operaciones elementales para estimar cuEstopara estimar cuántos pasos se requieren.
Esto ayuda a calcular su complejidad temporal .
Aunque una operación elemental siempre se considera como una sola unidad de tiempo , su cantidad total puede crecer con el tamaño de la entrada.
Por eso, al analizar algoritmos, se estudia cuántas operaciones elementales se ejecutan en total.

## POR QUÉ HAY QUE BUSCAR LA EFICIENCIA?

Buscar eficiencia en algoritmos significa encontrar soluciones que resen algoritmos significa encontrar soluciones que resuelvan problemas utilizando la menor cantidad posible de tiempo y recursos ( como memoria(como recuerdo).

Un algoritmo eficiente resuelve bien un problema , pero además lo hace rápido y con poco gasto computacional , incluso cuando trabaja con grandes cantidades de datos .
No es solo una buena práctica buscar la eficiencia, es una necesidad .
Permite crear programas más rápidos, más inteligentes y más útiles, especialmente en un mundo donde los datos crecen cada día más.

# Resumen de los libros Capitulo 3

# NOTACIÓN ASINTÓTICA INTRODUCCIÓN
## UNA NOTACIÓN PARA "EL ORDEN DE"
## OTRA NOTACIÓN ASINTÓTICA
## NOTACIÓN ASINTÓTICA CONDICIONAL
## NOTACIÓN ASINTÓNCA CON VARIOS PARÁMETROS
## OPERACIONES SOBRE NOTACIÓN ASINTÓTICA 
## PROBLEMAS
## REFERENCIAS Y TEXTOS MAS AVANZADOS
