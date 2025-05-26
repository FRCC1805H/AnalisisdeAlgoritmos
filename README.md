# AnalisisdeAlgoritmos
## Fecha 14/04/2025
## Nombre Fabian Cañar

# Lib Fundamentos de Algoritmia 

# Preliminares Semana 1 

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

### Cuantificadores

Los símbolos V y 3 se leen «para todo» y «existe», respectivamente. Para ilustrar esto, considérese un conjunto arbitrario X y una propiedad P sobre X. Escribimos (V x e X) IP (x)) para indicar que «todos los x de X tienen la misma propiedad P». De manera similar:
(5 x e X) [P (x)]
significa que «existe al menos un elemento de x en X que tiene la propiedad P».
Finalmente, escribiremos (9! x e X)IP (x)| para significar «existe exactamente un x en X que tiene la propiedad P». Si X es el conjunto vacío, (Vx e X) [P (x)] siempre es vacíamente verdadero,número natural mayor todavía. Cuando se utiliza la alternancia de cuantificadores, el orden en el cual se presentan los cuantificadores es importante. Por ejemplo, la afirmación (a m e N)Vn e N) (m> n 1 es evidentemente falsa: significaría que existe un entero m que es mayor que todos los números naturales (incluyendo el propio m).
Siempre y cuando el conjunto X sea infinito, resulta útil decir que no solamente existe un x e X tal que la propiedad de P (x) es cierta, sino que además existen infinitos de ellos. El cuantificador apropiado en este caso es 3.
Por ejemplo, ( = n e N) [n es primo]. Obsérvese que E es más fuerte que J pero más débil que V. Otro cuantificador útil, más fuerte que i pero todavía más débil que V, es V, que se usa cuando una propiedad es válida en todos los casos salvo posiblemente para un número finito de excepciones.
Por ejemplo, (Vn e N) [si n es primo, entonces n es impar] significa que los números primos siempre son impares, salvo posiblemente por un número finito de excepciones, en este caso hay solamente una excepción: 2 es a la vez primo y par.
Cuando estamos interesados en las propiedades de los números naturales, existe una definición equivalente para estos cuantificadores, y suele ser mejor pensar en ellos en consecuencia.

### Sumas y productos

En el caso en que n = 0, la suma se define como 0. Esto se generaliza en la fo
ma evidente para denotar una suma cuando i va desde m hasta n siempre cuando m sn + 1. En algunas ocasiones resulta útil considerar sumas condicio nales. Si P es una propiedad de los enteros,
TS (1)
denota la suma de f (i) para todos los enteros i tal que sea válido P (i). Esta suma puede no estar bien definida si involucra a un número infinito de enteros, podemos incluso utilizar una notación mixta.

### Miscelánea

Sin embargo, cuando x es negativo y no es un entero en sí x es más pequeño que este valor por una unidad. Por ejemplo, L-3½J = 4. De manera similar, definimos el techo de x, que se denota como Lx., como el menor entero que no es menor que x. Obsérvese que x - 1 < Lx ≤ x ≤|x|<x + 1 para todo x.
Si m ≥ 0 y n > 0 son enteros, m/n denota como siempre el resultado de dividir m por n, lo cual no es necesariamente un entero. Por ejemplo, 7/2 = 3½. Denotamos el cociente entero mediante el símbolo « =», por tanto 7 ÷ 2 = 3. For-malmente, m + n = Lm/n). También utilizamos mod para denotar el operador
«módulo» que se define , En otras palabras, m mod n es el resto cuando m es dividido por n.
Si m es un entero positivo, denotamos el producto de los m primeros enteros
positivos como m!, lo cual se lee factorial de m. Es natural definir 0! = 1. Ahora
bien n! = n x (n - 1)! para todos los enteros positivos n. Una aproximación útil del factorial es la que da la fórmula de Stirling: n ! = V2m n (n/e)", en donde e es la base de los logaritmos naturales.
Sin y r son enteros tales que 0≤Sn, se representa mediante ()el número de formas de seleccionar r elementos de un conjunto de cardinalidad n, sin tener en cuenta el orden en el cual hagamos nuestras.

## TÉCNICA DE DEMOSTRACIÓN 1: CONTRADICCIÓN

Ya hemos visto que puede existir toda una selección de algoritmos disponibles cuando nos preparamos para resolver un problema. Para decidir cuál es el más adecuado para nuestra aplicación concreta, resulta crucial establecer las propiedades matemáticas de los diferentes algoritmos, tal como puede ser el tiempo de ejecución como función del tamaño del ejemplar que haya que resolver. Esto puede implicar demostrar estas propiedades mediante una demostración matemáti-ca. Esta sección y la siguiente revisan dos técnicas de demostración que suelen ser útiles en Algoritmia: la demostración por contradicción y la demostración por inducción matemática.
La demostración por contradicción, que también se conoce como prueba indirec-ta, consiste en demostrar la veracidad de una sentencia demostrando que su negación da lugar a una contradicción. En otras palabras, supongamos que se desea demostrar la sentencia S. Por ejemplo, S podría ser «existe un número infinito de números primos». Para dar una demostración indirecta de S, se empieza por suponer que S es falso (o, equivalentemente, suponiendo que «no S» es verdadero). ¿Qué se puede deducir si, a partir de esa suposición, el razonamiento matemático establece la veracidad de una afirmación que es evidentemente falsa? Naturalmente, podría ser que el razonamiento en cuestión estuviera equivocado.

### Demostración

Sea P el conjunto de los números primos. Supongamos para buscar una tradicción que P es un conjunto finito. El conjunto P no es vacío, porque contiene al : nos el entero 2. Dado que P es finito y no está vacío, tiene sentido multiplicar todos: elementos. Sea x ese producto, y sea y el valor x + 1. Consideremos el menor entero que es mayor que 1 y que es el divisor de y. Este entero existe ciertamente por cuanto es mayor que 1 y no exigimos que d sea distinto de y. Obsérvese en primer lugar que en sí es primo, porque en caso contrario todo divisor propio de d dividiría también a y y sería más pequeño que d, que estaría en contradicción con la definición de d. (¿Ha observado el lector que la sentencia anterior es, en sí misma, una demostración por con-tradicción, anidada en el esquema general?) Por tanto, de acuerdo con nuestra suposición de que P contiene absolutamente todos los números primos, d pertenece a P. Esto demuestra que d es también divisor de x, puesto que x es el producto de una colección de enteros que contiene a d. Hemos llegado a la conclusión de que d divide exactamente tanto a x como a y. Pero se recordará que y = x + 1. Por tanto, hemos obtenido un entero d más grande que l y que divide a dos enteros consecutivos x e y. Esto es claramente imposible: si realmente d divide a x, entonces la división de y por d dejará necesariamente 1 como resto.

## TÉCNICA DE DEMOSTRACIÓN 2: INDUCCIÓN MATEMÁTICA

Las herramientas matemáticas básicas útiles en la Algoritmia, quizá no haya ninguna más importante que la inducción matemática. No sólo nos permite demostrar propiedades interesantes acerca de la correccióniy eficiencia de los al-goritmos, sino que además veremos en la Sección 1.6.4 que puede incluso utilizarse para determinar qué propiedades es preciso probar.
Antes de discutir la técnica, se ha de indicar una digresión acerca de la naturaleza del descubrimiento científico. En la ciencia hay dos enfoques opuestos fundamentales: inducción y deducción. De acuerdo con el Concise Oxford Dictio-nary, la inducción consiste en «inferir una ley general a partir de casos particu-lares», mientras que una deducción es una «inferencia de lo general a lo par-ticular». Veremos que, aun cuando la inducción puede dar lugar a conclusiones falsas, no se puede despreciar. La deducción, por otra parte, siempre es válida con tal de que sea aplicada correctamente.

### El principio de inducción matemática

Considérese el algoritmo siguiente:
función cuadrado (n)
Si n = 0 entonces devolver 0
Si no devolver 2n + cuadrado (n - 1) - 1 •
Si se prueba con unas cuantas entradas pequeñas, se observa que:
cuadrado (0) = 0, cuadrado (1) = 1, cuadrado (2) = 4, cuadrado (3) = 9, cuadrado (4) = 16
Por inducción, parece evidente que cuadrado (n) = n' para todos los n ≥ 0, ¿pe-ro cómo podría demostrarse esto rigurosamente? ¿Será verdad? Diremos que el algoritmo tiene éxito sobre el entero n siempre que cuadrado (n) = n2 y que fracasa en caso contrario.
Considérese cualquier entero n 2 1 y supóngase por el momento que el algoritmo tiene éxito en n -1. Por definición del algoritmo cuadrado (n) = 2n + cuadrado (n -1) -1. Por nuestra suposición cuadrado (n -1) = (n -1). Por tanto:
cuadrado (n) = 2n + (n - 1)2 - 1 = 2n + (n2 - 2n + 1) - 1 = n2
¿Qué es lo que hemos conseguido? Hemos demostrado que el algoritmo debe tener éxito en n siempre que tenga éxito en n - 1, siempre y cuando n ≥ 1.
Además está claro que tiene éxito en n = 0.
El principio de inducción matemática, que se describe más adelante, nos permite inferir a partir de lo anterior que el algoritmo tiene éxito en todos los n ≥ 0. Hay dos formas de comprender por qué se sigue esta conclusión: de forma constructiva y por contra-dicción.

### Un asunto completamente distinto

En cada uno de estos dos nuevos conjuntos hay n- 1 caballos. Por tanto, la hipótesis de inducción es aplicable a ellos. En particular, todos los caballos de H, son del mismo color, digamos cy y todos los caballos de H, son también de un único (posiblemente distinto) co-lor, digamos c, Pero ¿es realmente posible que el color c, sea diferente del color c? Ciertamente no, el caballo h, pertenece a los dos conjuntos por tanto ambos, c, y c,, deben ser del mismo color que el de dicho caballo! Como todos los caballos de H pertenecen a cualquier
H, o H, (o a ambos), concluimos que todos son del mismo color c = c, = G. Esto completa
el paso de inducción y la demostración por inducción matemática.
Antes de seguir adelante, encuentre la falacia de la «demostración» anterior.
Si piensa que el problema es que nuestra hipótesis de inducción («todo conjunto de n- 1 caballos debe de contener solamente caballos de un mismo color») era
absurda, ¡piénselo de nuevo!
Solución: El problema es que «h, pertenece a ambos conjuntos» no es cierto para
n = 2, ipuesto que h, no pertenece a H2! Nuestro razonamiento era impecable para
los casos básicos n = 0 y n = 1. Además, es cierto que nuestro teorema es consecuencia válida para los conjuntos de n caballos, suponiendo que sea válido para n - 1, pero solamente cuando n ≥ 3. Podemos pasar de 2 a 3 y de 3 a 4, y así sucesivamente, pero no de 1 a 2. Dado que los casos básicos son únicamente 0 y 1, y puesto que no podemos pasar de 1 a 2, el paso de inducción no puede comenzar. Este pequeño eslabón perdido dentro de la demostración basta para hacerla completamente inadmi-sible. Encontramos una situación similar al demostrar que n' < 2": el paso de inducción no era aplicable para n < 5, y por tanto la veracidad de la afirmación para n = 0
y p= anto alevante, la pife endis in votante en que de 2' es cierto para = 10.\

### Inducción matemática generalizada

El principio de inducción matemática descrito hasta el momento es adecuado para de mostrar muchas afirmaciones interesantes. Existen algunos casos, sin embargo, en los cuales es preferible un principio algo más potente. Se conoce con el nombre de inducción matemática generalizada. La situación se ilustra mediante el ejemplo siguiente:
Supongamos que se desea demostrar que todo entero compuesto se puede expresar como un producto de números primos. (El teorema fundamental de la aritmética nos dice que esta descomposición es única; esto no es lo que estamos intentando demostrar aquí.) No nos vamos a preocupar todavía por las bases de la inducción matemática, sino que vamos a saltar directamente al paso de induc-ción. Cuando se intenta demostrar que n se puede expresar como un producto de números primos (suponiendo que sea compuesto), la hipótesis de inducción «na-tural» sería que también se puede descomponer de esta manera n - 1. Sin em-bargo, desafiamos al lector a que encuentre algo en la descomposición de n - 1 en números primos que pueda ser útil o relevante para la descomposición de n en primos. Lo que se necesita realmente es una hipótesis de inducción más fuer-te, consistente en que todo número compuesto entero menor que n se puede descomponer en un producto de números primos. La demostración correcta de nuestro teorema se da más adelante como teorema 1.6.3, después de expresar formalmente el principio de inducción matemática generalizada.
Otra generalización útil concierne a la base.

### Inducción constructiva

La inducción matemática se utiliza sobre todo como técnica de demostración. Con harta frecuencia, se utiliza para demostrar afirmaciones que parecen haber surgido de la nada, como quien saca un conejo de un sombrero. Aunque la veracidad de tales afirmaciones queda comprobada, su origen sigue siendo un misterio. Sin embargo, la inducción matemática es una herramienta tan potente que nos permite no sólo descubrir meramente la veracidad de un teorema, sino también su enunciado exacto. Al aplicar la técnica de inducción constructiva que se describe en esta sección, puede uno demostrar simultáneamente la veracidad de una afirmación hecha de forma imprecisa y también descubrir las especificaciones omitidas, gracias a las cuales es correcta esa afirmación. Ilustraremos esta técnica mediante dos ejemplos que hacen uso de la sucesión de Fibonacci que se define más adelante. El segundo ejemplo muestra la forma en que esta técnica puede resultar útil para el análisis de algoritmos.

## RECORDATORIOS

En esta sección recordamos al lector algunos resultados elementales acerca de lí-mites, sumas de series sencillas, combinatoria y probabilidad. Los capítulos posteriores utilizarán las proposiciones que se presentan aquí.

### Límites 

Hay una definición parecida para fórmulas tales como -n ,
', que pueden tomar
valores negativos cada vez más grandes a medida que n tiende a infinito. Se dice que estas funciones tienden a menos infinito.
Por último, cuando f(n) no tiende a un límite, ni tampoco a +∞ o -0o, diremos que f(n) oscila cuando n tiende a infinito. Si es posible encontrar una constante positiva K tal que -K < f(n) < K para todos los valores de n, diremos que f(n) oscila de forma finita; en caso contrario, f(n) oscila de forma infinita. Por ejemplo, la función (-1)" oscila de forma finita; la función (-1)"n oscila de forma infinita.
Las proposiciones siguientes enuncian algunas de las propiedades generales.

### Series sencillas

Hay una definición parecida para fórmulas tales como -n", que pueden tomar valores negativos cada vez más grandes a medida que n tiende a infinito. Se dice que estas funciones tienden a menos infinito.
Por último, cuando f(n) no tiende a un límite, ni tampoco a +∞ o -∞, diremos que f(n) oscila cuando n tiende a infinito. Si es posible encontrar una constante positiva K tal que -K < f(n) < K para todos los valores de n,Idiremos que f(n) oscila de forma finita; en caso contrario, f(n) oscila de forma infinita. Por ejemplo, la función (-1)" oscila de forma finita; la función (-1)"n oscila de forma infinita.
Las proposiciones siguientes enuncian algunas de las propiedades generales de
los límites.

### Combinatoria básica

En este caso diremos que la serie es convergente, y llamaremos a s la suma de la serie.
Si por otra parte s, no tiende a un límite, sino que s, tiende a to o a -co, entonces diremos que la serie diverge, a too o quizá a -∞. Finalmente, si s, no tiende a un límite, ni a to ni a-co, entonces diremos que la serie oscila (de forma finita o quizá infinita). Es evidente que una serie que no tenga términos negativos debe de converger, o bien diverger, a +o: no podrá oscilar.
Dos clases de series especialmente sencillas son las series aritméticas y las series geométricas.

### Probabilidad elemental

Supongamos que se tienen n objetos que son suficientemente distintos para que podamos reconocer cada uno: diremos que estos objetos son distinguibles. Para facilitar la exposición supongamos que están rotulados con las letras a, b, y así sucesivamente, teniendo cada objeto un rótulo distinto. De ahora en adelante aludiremos simplemente a a, por ejemplo, cuando queramos decir «el objeto cuyo rótulo es a».
Nuestra primera definición concierne al número de formas en que se pueden
ordenar estos n objetos.

# ALGORITMIA ELEMENTAL Semana 2

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


# NOTACIÓN ASINTÓTICA  Semana 3
Esta notación se denomina «asintótica» porque trata acerca del comportamiento de funciones en el límite, esto es, para valores suficientemente grandes de su pa-rámetro. En consecuencia, los argumentos basados en la notación asintótica pueden no llegar a tener un valor práctico cuando el parámetro adopta valores « de la vida real». Sin embargo, las enseñanzas de la notación asintótica suelen tener una relevancia significativa. Esto se debe a que, como regla del pulgar, un algoritmo que sea superior asintóticamente suele ser (aunque no siempre) preferible incluso en casos de tamaño moderado.

## UNA NOTACIÓN PARA "EL ORDEN DE"

Aun cuando es natural utilizar el símbolo «» de teoría de conjuntos para denotar que n' es del orden de i' tal como en «n' e O (n3)», le advertimos que la notación tradicional es n? = O (17'). Por tanto, no se sorprenda si encuentra una de estas «igualdades» de un solo sentido, porque uno nunca escribiría O (n") = 1ª, en otros libros o artículos científicos. Aquellos que utilizan las igualdades de un solo sentido dicen que 12 es del orden de (o algunas veces sobre el orden de) n', o bien que n'es O (n*). Otra diferencia significativa que se puede encontrar en la definición de la notación O es que algunos escritores permiten que O (f(n)) incluya las funciones de los números naturales en el conjunto de todos los enteros reales
—incluyendo los reales negativos— y definen que una función está en O (f(n)) si
su valor absoluto está en lo que nosotros llamamos O (f(n)).
Por comodidad, nos permitiremos utilizar incorrectamente la notación de vez en cuando (así como otra notación que se presenta más adelante en este capítulo).
Por ejemplo, podemos decir que t(n) está en el orden de f(n) incluso si f(n) es negativo o no está definido para un número finito de valores de n. De manera simi-lar, podemos hablar acerca del orden de f(n) incluso en el caso de que f(i) sea negativa o no esté definida para un número finito de valores de n. Diremos entonces que t(n) e O (f(ir)) si existe una constante real y positiva c y un umbral entero n, tales que tanto (i) como f(il) están bien definidos y 0 ≤ t(n) ≤ cf(n) siempre que ≥ 11, independientemente de lo que suceda en estas funciones cuando n < ". Por ejemplo, está permitido hablar del orden de n/log i, aun cuando esta función no está definida cuando n = 0 ó n1 = 1, y es correcto escribir 1'-3n*-11-8 € O(n*) aun cuando n°- 3n2- 11-8 < 0 cuando n ≤ 3.

## OTRA NOTACIÓN ASINTÓTICA

Dado que ningún ejemplar de tamaño n puede tomar más tiempo que el tiempo máximo requerido por los ejemplares de ese tamaño, se sigue que la implementación requiere un tiempo acotado por cf(i) microsegundos para todos los ejemplares suficientemente grandes. Suponiendo que solamente exista un número finito de ejemplares de tamaño, puede haber solamente un número finito de ejemplares, todos ellos de tamaño menor que el umbral, sobre los cuales la implementación requiera un tiempo mayor que cf(i1) microsegundos. Suponiendo que f(i) nunca sea cero, todos éstos se pueden resolver utilizando una constante multiplicativa mayor, tal como se hace en la demostración de la regla del umbral.
Por contraste, supongamos que (n) € Q(f(n)). Una vez más, esto significa que existe una constante real positiva d tal que t(1) ≥ df(n) para todo n suficientemente grande. Ahora bien, dado que t(i) denota el comportamiento de esa implementación en el caso peor, podemos inferir solamente que, para cada i suficientemente grande, existe al menos il ejemplar de tamaño i1 tal que la implementación requiere al menos df(i) microsegundos para ese ejemplo. Esto no excluye la posibilidad de un comportamiento mucho más rápido sobre otros ejemplares del mismo tamaño. Por tanto, pueden existir infinitos ejemplares en los cuales la implementación requiera menos de df(n) microsegundos. La ordenación por inserción ofrece un ejemplo típico de este comportamiento. Vimos en la Sección 2.+ que se requiere un tiempo cuadrático en el caso peor, pero sin embargo existen infinitos ejemplares en los cuales se ejecuta en un tiempo lineal. Por tanto, tenemos derecho a manifestar que el tiempo de ejecución en el caso peor está tanto en O(172) como en S2(11*).

## NOTACIÓN ASINTÓTICA CONDICIONAL

Es eventualmente no decreciente —y por tanto, que no es uniforme porque
b(2' - 1) = k mientras que b(2*) = 1 para todo k. Sin embargo, f(n) e O (logn), que
es una función uniforme. (Este ejemplo no es tan artificial como pudiera parecer; véase la Sección 7.8.) En raras ocasiones se encontrarán funciones de crecimiento lento que no estén en el orden exacto de una función suave.
Una propiedad útil de la uniformidad (ajuste o suavización) es que si f es b-uni-forme para algún entero concreto b ≥ 2, entonces, de hecho, es uniforme. Para demostrar esto, considérense dos enteros cualesquiera a y b mayores o iguales que 2 Supongamos que f es b-uniforme. Debemos demostrar que j es también a-uniforme.
Sean c y no constantes tales que f (bil) ≤ c f (n) y f (1) ≤f (u + 1) para todo n ≥ 11o. Sea i = [log, al. Por definición del logaritmo, a = bosy ≤ blog = b Considérse cualquier n ≥ 0. Es fácil mostrar por inducción matemática sobre la b-uniformidad de f que f (b' n) ≤ c f (11). Pero f (an) ≤ f (b' n) (porque f es asintomáticamente no decreciente y b'n ≥ an ≥ no. Se sigue que f (an) ≤ô f (n) para ^ = c', y por tanto f es a-uniforme Las funciones uniformes son interesantes como consecuencia de la regla de la uniformidad (ajuste o suavidad). Sea f: 1 *→:2 una función suave y sea t:.. →. una función asintóticamente no decreciente. Considérese cualquier entero / ≥ 2.

## NOTACIÓN ASINTÓTICA CON VARIOS PARÁMETROS 

Puede suceder, cuando se analiza un algoritmo, que su tiempo de ejecución de penda simultáneamente de más de un parámetro del ejemplar en cuestión. Esta situación es típica de ciertos algoritmos para problemas de grafos, por ejemplo, en los cuales el tiempo depende tanto del número de nodos como del número de aris-tas. En tales casos la noción «tamaño del ejemplar» que se ha utilizado hasta el mo-mento, puede perder gran parte de su significado. Por esta razón, se generaliza la notación asintótica de forma natural para funciones de varias variables.
Sea f: 1'xIi→: «' una función de parejas de números naturales en los reales no negativos, tal como fin, n1) = m log n. Sea f: 1i x -"→":» otra función de éstas. Diremos que t(m, i1) es del orden de f(n, i), lo cual se denota Mm, i1) e O(f(n, i)) si /(in, n) está acotada superiormente por un múltiplo positivo de f(m, in) siempre que tanto in como ll sean suficientemente grandes.

### OPERACIONES SOBRE NOTACIÓN ASINTÓTICA

Para simplificar algunos cálculos, podemos manipular la notación asintótica empleando operadores aritméticos. Por ejemplo, O(fm)) + O(g(n)) representa el conjunto de operaciones abtenidas sumando punto a punto toda función de O (f(n)) a cualquier función de O(g(n1)). Intuitivamente este conjunto representa el orden del tiempo requerido por un algoritmo compuesto por una primera fase que requiere un tiempo del orden de f(i) seguido por una segunda fase que requiera un tiempo del orden de g(i1). Hablando con propiedad, las constantes ocultas que multiplican a f(n) y g(n) pueden muy bien ser distintas, pero esto no tiene importancia porque es sencillo demostrar que O(f(1)) + O(g(i1)) es idéntico a O(f(n) + g(i1)). Por la regla del máximo, sabemos que esto también es lo mismo que
O(máx(f(i), g(i1))) y, si se prefiere, máx(O(f(i1)), O(g(11))).

## ANÁLISIS DE ALGORITMOS Semana 4 

El objetivo principal de este libro es enseñarle a diseñar sus propios algoritmos efi-cientes. Sin embargo, cuando uno se enfrenta con varios algoritmos distintos para resolver el mismo problema, es preciso decidir cuál de ellos es el más adecuado para la aplicación considerada. Una herramienta esencial para este propósito es el análisis de algoritmos. Sólo después de haber determinado la eficiencia de los distintos algoritmos será posible tomar una decisión bien informada. Pero no hay una fórmula mágica para analizar la eficiencia de los algoritmos. En su mayor parte, es una cuestión de juicio, intuición y experiencia. Sin embargo, existen algunas técnicas básicas que suelen resultar útiles, tales como saber la forma de enfrentarse a estructuras de control y a ecuaciones de recurrencia.

## ANÁLISIS DE LAS ESTRUCTURAS DE CONTROL  

Además este tiempo está, claramente, acotado inferiormente por mt. Si c es despreciable en comparación con t, entonces nuestra estimación anterior de / como
aproximadamente igual a mt queda justificada, salvo por un caso crucial: / = mt
es completamente incorrecto cuando m = 0 (¡resulta incluso peor cuando m es ne-gativo!). Veremos en la Sección 4.3 que despreciar el tiempo necesario para el control del bucle puede dar lugar a graves errores en tales circunstancias.
Resista la tentación de decir que el tiempo requerido por el bucle está en
O(mt) con el pretexto de la notación © sólo tiene efecto más allá de algún umbral tal como m ≥ 1. El problema de este argumento es que si estamos realmente analizando todo un algoritmo y no simplemente el bucle para, entonces el umbral implícito en la notación © concierne a i, el tamaño del caso, y no a mi, el número de veces que pasamos por el bucle, y m = 0 podría suceder para valores arbitrariamente grandes de . Por otra parte, siempre y cuando t esté acotado inferiormente por alguna constante (lo cual siempre es cierto en la práctica), y siempre y cuando exista un umbral », tal que m ≥ 1 siempre que i1 2 11, el problema 4.3 pide demostrar que ‹ está ciertamente en ®(mt) cuando /, m y t se consideran como funciones de n.

### Secuencias

Sean P, y P, dos fragmentos de un algoritmo. Pueden ser instrucciones individuales o bien subalgoritmos complicados. Sean /, y t, los tiempos requeridos por P, y P, respectivamente. Estos tiempos pueden depender de distintos parámetros, tales como el tamaño del caso. La regla de la composición secuencial dice que el tiempo necesario para calcular "P; P,", esto es, primero P, y después P,, es simplemente t, + 1,. Por la regla del máximo este tiempo está en O(máx (f, (,).
A pesar de su sencillez, la aplicación de esta regla puede ser menos fácil de lo que parece en principio. Por ejemplo, puede ser que uno de los parámetros que controlan / dependa del resultado del cálculo efectuado por P,. Por tanto, el análisis de "P,; P,'
" no siempre se puede efectuar considerando P, y P, independientemente.

### Bucles "para" (desde).

Tanto aquí como en el resto del libro adoptamos el convenio de que n1 = 0 no es un error; significa simplemente que la instrucción controlada P(i) no se ejecuta ni una sola vez. Supongamos que este bucle es parte de un algoritmo más extenso, que trabaja en un ejemplar deitamaño 1. (Tenga cuidado para no confundir i con m.) El caso más sencillo es aquel en el cual el tiempo requerido por P(i) no depende realmente de i, aun cuando pudiera depender del tamaño del ejemplar o, más general-mente, del ejemplar en sí. Supongamos que t denota el tiempo requerido para calcular P(i). En este caso, el análisis evidente del bucle es que P(i) se efectúa m ve-ces, cada una de las cuales tiene un coste f, y por tanto el tiempo total requerido por
el bucle es simplemente / = mt. Aun cuando este enfoque suele ser apropiado, existe un posible problema: no hemos tenido en cuenta el tiempo necesario para el control del bucle.

### Llamadas recursivas

Si contamos las sumas con coste unitario, h(m) está acotado por una constante, y la ecuación de recurrencia para T(i1) es muy similar a la que ya hemos encontrado para g(i) en la Sección 1.6.4. La inducción constructiva se aplica igualmente bien para alcanzar la misma conclusión: T(i) e O(f,). Sin embargo, es más sencillo en este caso aplicar la técnica de la Sección 4.7 para resolver la recurrencia 4.1.
Un razonamiento similar muestra que T(i1) e Q(f,), y por tanto T(n) e O(f,). Empleando la fórmula de Moivre, concluimos que fibrec(n) requiere un tiempo exponencial en 1. Es decir doblemente exponencial en el tamaño del caso, puesto que el valor de i es exponencial en el tamaño de 1.
Si no se cuentan las adiciones con un coste unitario, /(i1) ya no queda acotado por una constante. En lugar de ocurrir esto, l(1) está dominado por el tiempo requerido para la adición de f.L, Y f, 2 para i suficientemente grande. Ya hemo- ris-to que esta adición requiere un tiempo que es del orden exacto de 1. Por tanto /z(m1) e ©(i1). Las técnicas de la Sección 4.7 son aplicables una vez más para resolver la recurrencia 4.1. Sorprendentemente, el resultado es el mismo independientemente de si h() es constante o lineal: sigue sucediendo que T(I) e O(f). En conclu-sión, Fibrec(n) requiere un tiempo exponencial en i1 (tanto si se cuentan las adiciones con coste unitario como si no!). La única diferencia es la constante multi-plicativa oculta en la notación (-).\

### Bucles "mientras" y "repetir"

Los bucles mientras (while) y repetir (repeat) suelen ser más difíciles de analizar que los bucles para (for), porque no existe una forma evidente a priori de saber cuántas veces tendremos que pasar por el bucle. La técnica estándar para analizar estos bucles es hallar una función de las variables implicadas cuyo valor se decremente en cada pasada. Para concluir que el bucle terminará por acabar, basta con saber que este valor debe ser un entero positivo. (No se puede seguir de-crementando indefinidamente un mínimo natural.) Para determinar el número de veces que se repite el bucle, sin embargo, necesitamos conocer mejor la forma en que disminuye el valor de esta función. Una aproximación alternativa al análisis del bucle mientras consiste en tratarlo como un algoritmo recursivo. Ilustraremos ambas técnicas con el mismo ejemplo. El análisis de bucles repetir se efectúa de manera similar; no daremos ejemplos de ellos en esta sección.
Estudiaremos con detalle la búsqueda binaria en la Sección 7.3. Sin embargo, la utilizamos ahora porque ilustra perfectamente el análisis de los bucles mientras.
El objetivo de la búsqueda binaria es hallar un elemento x de un vector /(l..n) que está ordenado de modo no decreciente. Supongamos por sencillez que está garantizado que x aparece al menos una vez en T.

## USO DE UN BARÓMETRO

El análisis de muchos algoritmos se simplifica de forma significativa cuando es posible aislar una instrucción —o una comprobación— como barómetro. Una "ins-trucción barómetro" es aquella que se ejecuta por lo menos con tanta frecuencia como cualquier otra instrucción del algoritmo. (No pasa nada si algunas instrucciones se ejecutan como mucho un número constante de veces más que el baró-metro, puesto que su contribución quedará absorbida en la notación asintótica.)
Siempre que el tiempo requerido por cada instrucción esté acotado por una cons-tante, el tiempo requerido por el algoritmo completo es del orden exaclo del número de veces que se ejecuta la instrucción barómetro.
Este enfoque resulta útil porque nos permite despreciar los tiempos exactos que requieren las distintas instrucciones. En particular, evita la necesidad de tener que introducir constantes tales como las que acotan el tiempo requerido por las distintas operaciones elementales, que carecen de significado puesto que dependen de la implementación, y se descartan cuando se expresa el resultado final en términos de la notación asintótica. Por ejemplo, considérese el análisis de Fibiter en la Sección 4.2.2 si contamos todas las operaciones aritméticas como de coste unitario. Vimos que el algoritmo requiere un tiempo acotado superior por en para alguna constante c carente de significado, y por tanto requiere un tiempo que está en O(i).

### Operacion de Inserccion 

A diferencia de la ordenación por selección, se vio en la Sección 2.4 que el tiempo necesario para ordenar n objetos por inserción depende significativamente del orden original de los elementos. Aquí analizamos este algoritmo en el caso peor; el análisis del caso medio se da en la Sección 4.5. Para analizar el tiempo de ejecución de este algoritmo, seleccionamos como barómetro el número de veces que se comprueba la condición (j > 0 y x < TIj)) del bucle mientras.
Consideremos un valor fijo de i. Sea x = T[i), como en el algoritmo. El caso
peor surge cuando x es menor que TUl para todo j entre 1 e/-2, puesto que en este caso tenemos que comparar x con Tli - 11, Tli - 21...., TIl antes de poder salir del bucle mientras, porque j = 0. Por tanto el bucle mientras se efectúa / veces en el caso peor. Este caso peor sucede para todos los valores de i entre 2 y 1 cuando el vector está ordenado inicialmente por orden decreciente. Entonces la comprobación del barómetro se efectúa 2,2 / = n (17 + 1)/2-1 veces en total, lo cual está en O(11ª).

### Algoritmos de Euclides 

Considérese lo que sucede con m y 1 después de pasar dos veces por el bucle, suponiendo que el algoritmo no se detenga antes. Supongamos que mu y 11, denotan el valor original de los parámetros. Después de la primera pasada por el bu-cle, m pasa a ser i1, mod mn. Después de la segunda pasada por el bucle, i toma ese valor. Por la observación anterior, » se ha vuelto más pequeño que 1o/2. En otras palabras, el valor de n se divide como mínimo por dos después de pasar dos veces por el bucle. En ese momento sigue siendo cierto que i ≥ m y por tanto vuelve a ser aplicable el mismo razonamiento: si el algoritmo no se ha detenido antes, otras dos pasadas por el bucle harán que el valor de n sea al menos dos veces más pequeño. Con cierta experiencia, la conclusión es ahora inmediata: en el bucle se va a entrar como máximo, aproximadamente, 2 lg 1 veces.
Formalmente, lo mejor es completar el análisis del algoritmo de Euclides tratando al bucle mientras como si fuese un algoritmo recursivo. Sea f(() el máximo número de veces que el algoritmo pasa por el bucle con unas entradas m y i cuando es m ≤ 11 ≤ 1. Si n ≤ 2, pasamos por el bucle o bien cero veces (si m = 0) o bien una vez. En caso contrario, o bien pasamos por el bucle menos de dos veces (si 171
= 0 ó m divide a i exactamente), o al menos dos veces.

### Las Torres de Hanoi

Las Torres de Hanoi nos ofrecen otro ejemplo del análisis de algoritmos recur-sivos. Se dice que después de crear el mundo, Dios puso en la tierra tres barras hechas de diamantes y 64 anillos de oro. Estos anillos son todos ellos de distintos tamaños. En la creación, se dispusieron en la primera barra por orden de tamaños, con el mayor en la parte inferior y el menor en la parte superior. También creó Dios un monasterio junto a las barras. La tarea de los monjes durante su vida es trasladar todos los anillos a la segunda barra. La única operación permitida es trasladar un solo anillo de una barra a otra de tal manera que nunca se coloque un anillo encima de otro que sea menor. Cuando los monjes hayan finalizado su tarea, dice la leyenda, se acabará el mundo. Probablemente sea la profecía que ofrece más consuelo con respecto al fin del mundo, porque si los monjes se las arreglasen para mover un anillo por segundo, trabajando día y noche sin descansar ni cometer errores, ¡su trabajo no habría terminado 500.000 millones de años después de que empezaran! ¡Son más de 25 veces la edad estimada del Universo!
Es evidente que el problema se puede generalizar para un número arbitrario de anillos, n.

### Cálculo de determinantes

Otro ejemplo mas de análisis de la recursividad es el que concierne al algoritmo recursivo para calcular un determinante. Recuérdese que el determinante de una matriz n x n se puede calcular a partir de los determinantes de n matrices más peque-ñas, (n- 1) × (n- 1) que se obtienen borrando la primera fila y alguna columna de la matriz original. Una vez que se han calculado los n subdeterminantes, el determinante de la matriz original se calcula con mucha rapidez. Además de las llamadas re-cursivas, la operación dominante que se necesita consiste en crear las n submatrices cuyos determinantes es preciso calcular. Esto requiere un tiempo que está en ®(n°) si se implementa directamente, pero basta un tiempo ®(n) si se utilizan punteros en lugar de copiar elementos. Por tanto, el tiempo total t(n) que se necesita para calcular el determinante de una matriz n x n mediante el algoritmo recursivo está dado por la recurrencia t(n) = nt(n-1) + h(n) para n ≥ 2, donde h(n) € ®(n). Esta recurrencia no se puede tratar mediante las técnicas de la Sección 4.7. Sin embargo, vimos en el problema 1.31 que la inducción constructiva es aplicable para concluir que t(n) € ®(n!), lo cual muestra que este algoritmo es muy ineficiente.

## ANÁLISIS DEL CASO MEDIO

Esto requiere suponer a priori una distribución de probabilidad para los casos en que se pedirá que resuelva nuestro algoritmo. La conclusión del análisis en el caso medio puede depender crucialmente de esta suposición, y este análisis puede inducir a error si de hecho nuestras suposiciones no se corresponden con la realidad de la aplicación que utiliza el algoritmo. Este tema tan importante se discutía con más extensión en la Sección 2.4, y volveremos a él en la Sección
10.7. En la mayoría de las ocasiones, los análisis en el caso medio se efectúan haciendo la suposición (más o menos realista) consistente en que todos los ejemplares de un tamaño dado son igualmente probables. Para los problemas de ordena-ción, resulta más sencillo suponer también que todos los elementos que hay que ordenar son distintos.
Supongamos que se tienen que ordenar i elementos distintos por inserción, ! que las i! permutaciones de estos elementos son igualmente probables. Para determinar el tiempo requerido en el caso medio por el algoritmo, podríamos sumar los tiempos requeridos para ordenar todas y cada una de las permutaciones posibles y dividir entonces por n! la respuesta obtenida. Una aproximación alternati-va, más sencilla en este caso, consiste en analizar directamente el tiempo requerimiento.

## ANÁLISIS AMORTIZADO

En algunas ocasiones, el análisis del caso peor es excesivamente pesimista.
Considérese por ejemplo un proceso P que tiene efectos secundarios, lo cual significa que P modifica el valor de variables globales. Como resultado de los efectos secundarios, dos llamadas sucesivas e idénticas a P podrían requerir cantidades de tiempo radicalmente diferentes. Cuando se esté analizando un algoritmo que tenga a P como subalgoritmo, lo fácil sería analizar P en el caso peor, y suponer que sucede lo peor cada vez que se llama a P. Este enfoque produce una respuesta correcta suponiendo que estemos satisfechos con un análisis en notación O, por oposición a la notación ©, pero la respuesta sería pesimista. Considérese por ejemplo el bucle siguiente:
para i - 1 hasta i hacer P
Si P requiere un tiempo en O(log n) en el caso peor, es correcto concluir que el bucle requiere un tiempo en O(n log «), pero puede suceder que sea mucho más rápido incluso en el caso peor. Esto podría suceder si P no puede tardar mucho tiempo (S(logn)) a no ser que haya sido invocado muchas veces anteriormente, con un coste pequeño en todas las llamadas. Por ejemplo, podría suceder que P requiriera un tiempo constante en el caso medio, en cuyo caso el bucle completo se ejecutaría en un tiempo lineal.

## RESOLLCIÓN DE RECURRENCIAS

El último paso indispensable cuando se está analizando un algoritmo es frecuentemente la resolución de una ecuación de recurrencia. Con un poco de experiencia y de intuición, la mayoría de las recurrencias se puede resolver mediante suposiciones inteligentes. Sin embargo, existe una potente técnica que se puede utilizar para resolver de forma casi automática ciertas clases de recurrencias. Ese es el tema principal de esta sección: la técnica de la ecuación característica.

### Suposiciones inteligentes

Este enfoque suele desarrollarse en cuatro etapas: calcular los primeros valores de la recurrencia, buscar una regularidad, inventar una forma general adecuada y demostrar finalmente por inducción matemática (quizá por inducción construc-tiva) que esta forma es correcta.

### Recurrencias homogéneas

La situación se vuelve ligeramente más complicada cuando el polinomio característico tiene raíces múltiples, esto es, cuando las k raíces no son todas dife-rentes. Sigue siendo cierto que la Ecuación 4.8 satisface la recurrencia para valores cualesquiera de las constantes c, pero ésta ya no es la solución más general. Para hallar otras soluciones, sea p(x) = ax* + a,al + ... + a el polinomio característico de nuestra recurrencia, y sea r una raíz múltiple. Por definición de las rafces múl-
tiples, existe un polinomio q(x), de grado k-2, tal que p(x) = (x-r)2g(x). Para todo n
≥ k, considérense los polinomios de grado n.

### Recurrencias no homogéneas

Siempre y cuando t, ≥ 0, una sencilla demostración por inducción matemática basada en la ecuación 4.11 muestra que t,≥ 0 para todo n ≥ 0. Por tanto, resulta inmediato a partir de la ecuación 4.14 que t, € O(3"): no hay necesidad de resolver para las constantes c, y C, con objeto de alcanzar esta conclusión. Sin embargo, esta ecuación no basta por si misma para concluir que t, € 0(3") porque a priori podría ser c, = 0. Sin embargo, resulta que el valor de c, se puede obtener directa-mente, sin necesidad de construir el sistema 4.15 de ecuaciones lineales. Esto basta para concluir que t, € ©(3") independientemente del valor de t, (aun cuando sea negativo).

### Cambios de variable

A veces es posible resolver recurrencias más complicadas efectuando un cambio de variable. En los ejemplos siguientes, escribiremos T(n) para el término de una recurrencia general, y t, para el término de una nueva recurrencia obtenida a partir de la primera mediante un cambio de variable. Asegúrese de estudiar el Ejemplo 4.7.13, que se encuentra entre las recurrencias más importantes a efectos.

### Transformaciones de intervalo

Cuando se hace un cambio de variable, se transforma el dominio de la recu-rrencia. En lugar de hacer esto, puede resultar útil transformar el intervalo para obtener una recurrencia que tenga una forma que sepamos resolver. Ambas transde este enfoque.
formaciones pueden utilizarse a la vez en algunas ocasiones.

### Recurrencias asintóticas

Este tipo de ecuación se denomina recurrencia asintótica. Afortunadamente, la solución asintótica de una recurrencia tal como la ecuación 4.36 es prácticamente siempre idéntica a la forma de la ecuación 4.35, más sencilla. La técnica general para resolver una recurrencia asintótica consiste en "emparedar" la función que define entre dos recurrencias del tipo más sencillo. Cuando las dos recurrencias más sencillas tienen la misma solución asin-tótica, la recurrencia asintótica debe de tener también la misma solución.

## ESTRUCTURAS DE DATOS Semana 5

Sin embargo, este libro no pretende ser un manual de estructuras de datos. Suponemos que el lector ya posee buenos conocimientos prácticos de nociones tales como las matrices, los registros y los distintos tipos de datos estructurados que se obtienen empleando punteros. También suponemos que los conceptos matemáticos de grafos dirigidos y no dirigidos le resultan razonablemente familiares, y que el lector conoce la forma de representar eficientemente estos objetos en una computadora.

## MATRICES (ARRAYS), PILAS Y COLAS

Desde el punto de vista que nos interesa en este libro, la propiedad esencial de una matriz es que podemos calcular la dirección de cualquier elemento dado en un tiempo constante. Por ejemplo, si sabemos que la matriz anterior tab comienza en la dirección 5000, y que las variables enteras ocupan 4 bytes de almacenamiento cada una, entonces la dirección del elemento cuyo índice es k está dada claramente por 4996 + 4k. Aun cuando pensemos que merece la pena comprobar que k se encuentra realmente entre 1 y 50, el tiempo necesario para calcular la dirección sigue estando acotado por una constante. Se sigue que el tiempo necesario para leer el valor de un solo elemento, o para cambiar ese valor, se encuentra en O(1); en otras palabras, podemos tratar estas operaciones como si fuesen elementales.
Por otra parte, toda operación que implique a todos los elementos de una matriz tenderá a requerir más tiempo a medida que crezca el tamaño de la matriz. Supongamos que nos estamos enfrentando a una matriz de tamaño variable n; esto es, la matriz consta de i elementos. Entonces una operación tal como dar valor inicial a todos los elementos, o buscar el mayor elemento, va a requerir normalmente un tiempo que será proporcional al número de elementos que haya que examinar. En otras palabras, esas operaciones requieren un tiempo que está en O(i1).

## REGISTROS Y PUNTEROS (APUNTADORES)

Del mismo modo que una matriz tiene un número fijo de elementos del mismo tipo, un registro es una estructura de datos que consta de un número fijo de elementos, que suelen llamarse campos en este contexto, y que son de tipos posiblemente distintos. Por ejemplo, si la información acerca de una persona que nos interesa consta de nombre, edad, peso y sexo, quizá necesitemos utilizar.

## LISTAS

Las listas admiten un cierto número de operaciones: quizá sea necesario insertar un nodo adicional, borrar un nodo, copiar una lista, contar el número de elementos que contienen, y así sucesivamente. Las distintas implementaciones de computadora que se suelen utilizar difieren en la cantidad de espacio requerido, y en la facilidad para efectuar ciertas operaciones. Aquí nos contentaremos con mencionar las técnicas más conocidas.
Implementada en forma de matriz mediante la declaración.

## GRAFOS

Hablando intuitivamente, un grafo es un conjunto de nodos unidos por un conjunto de líneas o flechas. Considérese, por ejemplo, la figura 5.3. Distinguiremos entre grafos dirigidos y grafos no dirigidos. En los grafos dirigidos, los nodos están unidos mediante flechas llamadas aristas. En el ejemplo de la figura 5.3, existe una arista que va desde alfa hasta gamma, y otra desde gamma hasta alfa. Los nodos beta y delta, sin embargo, solo están unidos en la dirección indicada. En el caso de un grafo no dirigido, los nodos están unidos mediante líneas sin indicación de dirección, que también se llaman aristas. Tanto en los grafos dirigidos como en los no dirigidos, las secuencias de aristas pueden formar caminos y ciclos. Se dice que un grafo es conexo si se puede llegar desde cualquier nodo hasta cualquier otro siguiendo una secuencia de aristas; en el caso de un grafo dirigido, se permite circular en sentido inverso a lo largo de una flecha.

## ÁRBOLES

El árbol con raíz que se muestra en la figura 5.5 se representaría tal como en la figura 5.7, en la cual las flechas muestran la dirección de los punteros empleados en la representación por computadora, y no la dirección de las aristas del árbol (que es, por supuesto, un grafo no dirigido.) Insistimos en que esta representación se puede utilizar para cualquier árbol con raíz; tiene la ventaja de que todos los nodos se pueden representar utilizando la misma estructura registro, independientemente del número de hijos y hermanos que posean. Sin embargo, hay muchas operaciones que resultan ineficientes cuando se emplea esta representación míni-ma: no resulta evidente la forma de hallar el padre de un nodo dado.

## TABLAS ASOCIATIVAS

Una tabla asociativa es exactamente igual que una matriz, salvo que su índice no está restringido a encontrarse entre dos cotas predeterminadas. Por ejemplo, si T es una tabla, se puede utilizar 714] y después T[106) sin necesidad de reservar un millón de posiciones de almacenamiento para la tabla. Y aún hay algo mejor, se pueden utilizar cadenas en lugar de números como índice, así que T["Juan"] es tan legítimo como T[4]. Idealmente, una tabla no debería de ocupar mucho más espacio que el necesario para anotar los índices utilizados hasta el momento, junto al espacio para los valores almacenados en esas posiciones de la tabla.
La comodidad de las tablas tiene su precio: a diferencia de las matrices, las tablas no se pueden implementar de tal manera que se garantice que todas las búsquedas requieran un tiempo constante.

## MONTÍCULOS (HEAPS) 

Un montículo (heap) es un tipo especial de árbol con raíz que se puede implementar eficientemente en una matriz sin ningún puntero explícito. Esta estructura tan interesante se presta a numerosas aplicaciones, incluyendo una notable técnica de ordenación denominada ordenación por el método del montículo (heapsort), que se presentará más adelante en esta sección. También se puede utilizar para representar eficientemente ciertas listas dinámicas de prioridad, tales como la lista de sucesos en una simulación de una lista de tareas que haya de ser planificada por un sistema operativo.
Se dice que un árbol binario es esencialmente completo si todo nodo interno, con la posible excepción de un nodo especial, tiene exactamente dos hijos. El nodo es-pecial, si existe uno, está situado en el nivel 1, y posee un hijo izquierdo pero no tiene hijo derecho. Además, o bien todas las hojas se encuentran en el nivel 0, á bien están en los niveles cero y uno, y ninguna hoja del nivel 1 está a la izquierda de un nodo interno del mismo nivel. Intuitivamente, un árbol esencialmente completo es uno en el que los nodos internos se han subido en el árbol lo más posible. con los nodos internos del último nivel empujados hacia la izquierda; las hojas llenan el último nivel que contiene nodos internos, si es que queda algún espacio, y después se desbordan hacia la izquierda en el nivel cero.

## MONTÍCULOS BINOMIALES

En un montículo ordinario que contenga n elementos, buscar el mayor de ellos requiere un tiempo que está en O(1). Borrar el mayor elemento, o insertar un nuevo elemento, requiere un tiempo que está en O(log I). Sin embargo, fusionar dos montículos que contengan entre los dos it elementos requiere un tiempo que está en O(ii). En esta sección describiremos un tipo distinto de montículo, en el cual la búsqueda del mayor elemento sigue requiriendo un tiempo en O(1), y el borrado del mayor elemento sigue requiriendo un tiempo en Ollog i). Sin em-bargo, la fusión de dos de estos nuevos montículos sólo requiere un tiempo en O(log ), y la inserción de un nuevo elemento - siempre y cuando se considere el tiempo amortizado, y no el coste en si de cada operación- solamente requiere un tiempo en O(1).
Definiremos primero los árboles binomiales. El i-ésimo árbol binomial B, con i ≥ 0, se define recursivamente como aquel que consta de un nodo raíz con i hi-jos, en donde el j-ésimo hijo, 1 ≤ j <i, es a su vez la raíz de un árbol binomial
B, La figura 5.17 muestra desde B, hasta B. Es fácil mostrar por inducción matemática que el árbol binomial B, contiene 2' nodos, de los cuales están a una profundidad k, 0 ≤ k Si. Aqui; es el coeficiente binomial definido en la Sección 1.7.3. Esta es, por supuesto, la razón del nombre a los árboles binomiales.
Suponemos que todo nodo de estos árboles puede almacenar un valor. Dado que los nodos poseen un número variable de hijos, lo más probable es que la mejor manera de representarlos en una computadora sea utilizar.

## ESTRUCTURAS DE CONJUNTOS DISJUNTOS (PARTICIÓN)

Supongamos que vamos a ejecutar una secuencia arbitraria de operaciones de los tipos buscar y fusionar, comenzando a partir de la situación inicial. No sabemos precisamente el orden en que se van a producir estas operaciones. Sin embargo, habrá n del tipo buscar, y no habrá más de N-1 del tipo fusionar, porque al cabo de N-1 operaciones fusionar todos los objetos están en el mismo conjunto. Además, en muchas aplicaciones, n es comparable con N. Si la consulta o modificación de un elemento cuenta como una operación elemental, entonces está claro que buscarl requiere un tiempo constante, y que fusionarl requiere un tiempo que está en ©(N). Las n operaciones buscar, por tanto, requieren un tiempo en 0(7), mientras que las N-1 operaciones fusionar requieren un tiempo que está en O(N?). Si n y N son comparables, entonces toda la secuencia de operaciones requiere un tiempo que se encuentra en 0(12).
Intentemos hacerlo mejor. Sin dejar de utilizar una sola matriz, podemos representar cada conjunto como un árbol con raíz, en el cual cada nodo contiene un único puntero que apunta a su padre (tal como en el tipo nodoárbol2 de la Sección 5.5).
Adoptamos el convenio siguiente: si conjuntoli] = i, entonces i es a la vez el rótulo de su conjunto y la raíz del árbol correspondiente; si conjuntolil = j# i, entonces j es el padre de i en algún árbol.

## ALGORIIMOS VORACES Semana 6

Los algoritmos voraces se utilizan típicamente para resolver problemas de op-timización. Los ejemplos posteriores de este capítulo incluyen la búsqueda de la ruta más corta para ir desde un nodo a otro a través de una red de trabajo o la búsqueda del mejor orden para ejecutar un conjunto de tareas en una computadora.
En tales contextos, un algoritmo voraz funciona seleccionando el arco, o la tarea, que parezca más prometedora en un determinado instante; nunca reconsidera su decisión, sea cual fuere la situación que pudiera surgir más adelante. No hay necesidad de evaluar alternativas, ni de emplear sofisticados procedimientos de seguimiento que permitan deshacer las decisiones anteriores. Comenzaremos este capítulo con un ejemplo cotidiano en el que esta táctica funciona bien.

### DAR LA VUELTA (1) 

Los algoritmos voraces se utilizan típicamente para resolver problemas de op-timización. Los ejemplos posteriores de este capítulo incluyen la búsqueda de la ruta más corta para ir desde un nodo a otro a través de una red de trabajo o la búsqueda del mejor orden para ejecutar un conjunto de tareas en una computadora.
En tales contextos, un algoritmo voraz funciona seleccionando el arco, o la tarea, que parezca más prometedora en un determinado instante; nunca reconsidera su decisión, sea cual fuere la situación que pudiera surgir más adelante. No hay necesidad de evaluar alternativas, ni de emplear sofisticados procedimientos de seguimiento que permitan deshacer las decisiones anteriores. Comenzaremos este capítulo con un ejemplo cotidiano en el que esta táctica funciona bien.

### CARACTERÍSTICAS GENERALES DE LOS ALGORITMOS VORACES

A medida que avanza el algoritmo, vamos acumulando dos conjuntos. Uno contiene candidatos que ya han sido considerados y seleccionados, mientras que el otro contiene candidatos que han sido considerados y rechazados.
Existe una función que comprueba si un cierto conjunto de candidatos constituye una solución de nuestro problema, ignorando si es o no óptima por el mo-mento. Por ejemplo, ¿suman las monedas seleccionadas la cantidad que hay que pagar? ¿Proporcionan las aristas seleccionadas una ruta hasta el nodo que deseamos alcanzar? ¿Están planificadas todas las tareas?
Hay una segunda función que comprueba si un cierto conjunto de candidatos es factible, esto es, si es posible o no completar el conjunto añadiendo otros candidatos para obtener al menos una solución de nuestro problema. Una vez más, no nos preocupa aquí si esto es óptimo o no. Normalmente, se espera que el problema tenga al menos una solución que sea posible obtener empleando candidatos del conjunto que estaba disponible inicialmente.
Hay otra función más, la función de selección, que indica en cualquier momento cuál es el más prometedor de los candidatos restantes, que no han sido seleccionados ni rechazados.
Por último, existe una función objetivo que da el valor de la solución que hemos hallado: el número de monedas utilizadas para dar la vuelta, la longitud de la ruta que hemos construido, el tiempo necesario para procesar todas las tareas de la planificación, o cualquier otro valor que estemos intentando optimizar. A diferencia de las tres funciones mencionadas anteriormente, la función objetiva no aparece explícitamente en el algoritmo voraz.

### GRAFOS: ÁRBOLES DE RECUBRIMIENTO MÍNIMO

Sea G = (N, A) un grafo conexo no dirigido en donde N es el conjunto de nodos y
A es el conjunto de aristas. Cada arista posee una longitud no negativa. El problema consiste en hallar un subconjunto T de las aristas de G tal que utilizando solamente las aristas de T, todos los nodos deben quedar conectados, y además la suma de las longitudes de las aristas de T debe ser tan pequeña como sea posible.
Dado que G es conexo, debe existir al menos una solución. Si G tiene aristas de longitud 0, pueden existir varias soluciones cuya longitud total sea la misma, pero que tengan números distintos de aristas. En este caso, dadas dos soluciones de igual longitud total, preferimos la que contenga menos aristas. Incluso con esta condición el problema puede tener varias soluciones diferentes y de igual valor.
En lugar de hablar de las longitudes, podemos asóciar un coste a cada arista. El problema, entonces, consiste en hallar un subconjunto T de las aristas cuyo coste total sea el menor posible.

### Algoritmo de Kruskal

El conjunto de aristas T está vacío inicialmente. A medida que progresa el algo-ritmo, se van añadiendo aristas a T. Mientras no haya encontrado una solución, el grafo parcial formado por los nodos de G y las aristas de T consta de varios componentes conexos. (Inicialmente, cuando T está vacío, cada nodo de G forma una componente conexa distinta trivial) Los elementos de T que se incluven en una componente conexa dada forman un árbol de recubrimiento mínimo para los nodos de esta componente. Al final del algoritmo, sólo queda una componente cone-xa, así que T es un árbol de recubrimiento mínimo para todos los nodos de G.
Para construir componentes conexas más y más grandes, examinamos las aristas de G por orden creciente de longitudes.

### Algoritmo de Prim

Se vio anteriormente que el algoritmo de Kruskal requiere un tiempo que está en ©(a log i1), en donde a es el número de aristas que hay en el grafo. Para un grafo denso, a tiende a n(n - 1)/2. En este caso, el algoritmo de Kruskal requiere un tiempo que se encuentra en 0(nlog n), y el algoritmo de Prim puede ser mejor. Para un grafo disperso, a tiende a n. En este caso, el algoritmo de Kruskal requiere un tiempo que está en (n log n), y el algoritmo de Prim, tal como se ha presentado aquí, es probablemente menos eficiente. Sin embargo, el algoritmo de Prim, al igual que el de Kruskal, se puede implementar utilizando montículos. En este caso —una vez más, como el algoritmo de Kruskal— requiere un tiempo que está en ©(a log n). Existen otros algoritmos más eficientes que el de Prim o el de Kruskal.

## GRAFOS: CAMINOS MÍNIMOS

Considere ahora un grafo dirigido G = (N, A) en donde N es el conjunto de nodos
de G, y A es el conjunto de aristas dirigidas. Cada arista posee una longitud no ne-gativa. Se toma uno de los nodos como nodo origen. El problema consiste en determinar la longitud del camino mínimo que va desde el origen hasta cada uno de todos los demás nodos del grafo. Tal como sucedía en la Sección 6.3, podríamos hablar igualmente bien acerca del coste de una arista, en lugar de mencionar su longitud, y se podría plantear el problema consistente en determinar la ruta más barata desde el origen hasta cada uno de todos los demás nodos.
Este problema se puede resolver mediante un algoritmo voraz que recibe frecuentemente el nombre de algoritmo de Dijkstra. El algoritmo utiliza dos conjuntos de nodos, S y C. En todo momento, el conjunto § contiene aquellos nodos que ya han sido seleccionados; como veremos, la distancia mínima desde el origen ya es conocida para todos los nodos de S. El conjunto C contiene todos los demás nodos, cuya distancia mínima desde el origen todavía no es co-nocida, y que son candidatos a ser seleccionados en alguna etapa posterior. Por
tanto, tenemos la propiedad invariante N = SU C. En un primer momento, S
contiene nada más el origen en sí; cuando se detiene el algoritmo, S contiene todos los nodos del grafo y nuestro problema está resuelto. En cada paso seleccionamos aquel nodo de C cuya distancia al origen sea mínima.

## EL PROBLEMA DE LA MOCHILA (I)

Nuestro objetivo es llenar la mochila de tal manera que se maximice el valor de los objetos transportados, respetando la limitación de capacidad impuesta.
En esta primera versión del problema, suponemos que se pueden romper los objetos en trozos más pequeños, de Imanera que podamos decidir llevar solamente una fracción x, del objeto i, con 0 ≤ x, ≤ 1. (Si no se nos permite romper los objetos, el problema es mucho más difícil.) En este caso, el objeto i contribuye en x,u, al peso total de la mochila, y en x,o, al valor de la carga.

## PLANIFICACIÓN 

En esta sección presentamos dos problemas que conciernen a la forma óptima de planificar tareas en una sola máquina. En el primero, el problema consiste en minimizar el tiempo medio que invierte cada tarea en el sistema. En el segundo, las tareas tienen un plazo fijo de ejecución, y cada tarea aporta unos ciertos beneficios sólo si está acabada al llegar su plazo: nuestro objetivo es maximizar la rentabili-dad. Ambos problemas se pueden resolver empleando algoritmos voraces.

### Minimización del tiempo del sistema

Un único servidor, como por ejemplo un procesador, un surtidor de gasolina, o un cajero de un banco, tiene que dar servicio a n clientes. El tiempo requerido por cada cliente se conoce de antemano: el cliente i requerirá un tiempo t, para 1 si s n.
Deseamos minimizar el tiempo medio invertido por cada cliente en el sistema. Dado que el número n de clientes está predeterminado, esto equivale a minimizar el tiempo total invertido en el sistema por todos los clientes. En otras palabras, deseamos minimizar.

### Planificación con plazo fijo

Se dice que un conjunto de tareas es factible si existe al menos una sucesión (que también se llama factible) que permite que todas las tareas del conjunto se ejecuten antes de sus respectivos plazos. Un algoritmo voraz evidente consiste en construir la planificación paso a paso, añadiendo en cada paso la tarea que tenga el mayor valor de g, entre las que aún no se hayan considerado, siempre y cuando el conjunto de tareas seleccionadas siga siendo factible.
En el ejemplo precedente seleccionamos en primer lugar la tarea 1. Después tomamos la tarea 4; el conjunto (1, 4) es factible porque se puede ejecutar en el orden 4, 1. A continuación probamos el conjunto (1, 3, 4), que resulta no ser factible; por tanto se rechaza la tarea 3. Per último, probamos (1, 2, 4), que tampoco es fac-tible, así que se rechaza la tarea 2. Nuestra solución (que en este caso es óptima) es por tanto ejecutar el conjunto de tareas (1, 4), que sólo se puede efectuar en el orden 4, 1. Queda por demostrar que este algoritmo siempre encuentra una planificación óptima, y además hay que buscar una forma eficiente de implementarlo.

## DIVIDE Y VENCERÁS Semana 7

Divide y vencerás es una técnica para diseñar algoritmos que consiste en descomponer el caso que haya que resolver en un cierto número de subcasos más pequeños del mismo problema, resolver sucesiva e independientemente todos estos subcasos, y combinar después las soluciones obtenidas de esta manera para obtener la solución del caso original. Las dos preguntas que surgen de modo natural son: ¿por qué querría nadie hacer esto? y ¿cómo se resuelven los subcasos? La eficiencia de la técnica de divide y vencerás se debe a la respuesta a esta última pregunta.

## INTRODUCCIÓN: MULTIPLICACIÓN DE ENTEROS MUY GRANDES

Consideremos una vez más el problema de multiplicar enteros muy grandes.
Recordemos que el algoritmo clásico (figura 1.1) que aprendemos en la escuela requiere un tiempo en ©(n*) para multiplicar números de i cifras. Estamos tan acostumbrados a este algoritmo que quizá nunca haya tenido dudas acerca de su op-timalidad. ¿Podemos hacerlo mejor? La multiplicación à la russe (figura 1.2) no ofrece mejoras del tiempo de ejecución.
Lamentablemente, el algoritmo resultante no proporciona
ninguna mejora con respecto al algoritmo clásico de multiplicación, a no ser que seamos más inteligentes. Para superar al algoritmo clásico, debemos encontrar una forma de reducir la multiplicación original no a cuatro sino a tres multiplicaciones de números de tamaño mitad.

## EL CASO GENERAL

Algunos algoritmos de divide y vencerás no siguen exactamente este esquema: por ejemplo, pueden necesitar que el primer subejemplar esté resuelto antes de formular el segundo subejemplar; véase la Sección 7.5.
El número de subejemplares, ', suele ser pequeño e independiente del caso particular que haya que resolver. Cuando / = 1, no tiene mucho sentido «des-componer x en un caso más sencillo x,», y es difícil justificar el nombre de divide y vencerás que se le da a esta técnica. Sin embargo, tiene sentido reducir la resolución de un caso muy grande a la de uno más pequeño. Entonces, divide y vencerás recibe el nombre de reducción (simplificación); véanse las Secciones 7.3 y 7.7. Cuando se utiliza la simplificación, a veces es posible sustituir la recursi-vidad inherente a divide y vencerás por un bucle iterativo. Cuando se implementa en un lenguaje convencional como Pascal y en una máquina convencional que utilice un compilador poco sofisticado, un algoritmo iterativo tiene probabilidades de ser más rápido que la versión recursiva, aunque sólo por una constante multiplicativa. Por otra parte, puede ser posible ahorrar una cantidad considerable de memoria de esta manera: para un caso de tamaño it, el algoritmo recursivo utiliza una pila cuyo tamaño está en S2(lg n), y en casos ma-
los incluso en (n).

## BÚSQUEDA BINARIA

La búsqueda binaria precedió a las computadoras. En esencia, es el algoritmo que se emplea para buscar una palabra en un diccionario, o un nombre en un directorio telefónico. Probablemente se trate de la aplicación más sencilla de divide y vencerás, tan sencilla que hablando con propiedad esto es una aplicación de reducción (simplificación) más que de divide y vencerás: la solución de todo caso suficientemente grande se reduce a un caso más pequeño, en este caso de tamaño mitad.
Sea T[1...] una matriz ordenada por orden no decreciente; esto es, T(i] ≤ TU] siempre que sea 1s is js n. Sea x un elemento. El problema consiste en buscar x en la matriz T, si es que está. Formalmente, deseamos encontrar el índice i tal que 1 sisn + 1 y T[i - 1] < x ≤ T[], con la convención lógica consistente en que T[0] = -∞o y T[n + 1] = +o (al decir convenio lógico queremos indicar que estos valores no están realmente presentes en la matriz). La aproximación evidente para este problema consiste en examinar secuencialmente todos los elementos de T, hasta que o bien lleguemos al final de la matriz, o bien encontremos un elemento que no sea menor que x.

## ORDENACIÓN 

Sea T|l.n| una matriz de n elementos. Nuestro problema es ordenar estos elementos por orden ascendente. Ya hemos visto que el problema se puede resolver mediante ordenación por selección y ordenación por inserción (Sección 2.4), o bien mediante ordenación por montículo (Reapsort) (Sección 5.7). Recordemos que el análisis en los casos peor y promedio muestra que este último método requiere un tiempo que está en O(1 log n), mientras que los dos métodos anteriores requieren un tiempo cuadrático. Hay varios algoritmos clásicos de ordenación que siguen el esquema de divide y vencerás. Es interesante observar lo diferentes que son: aun habiendo decidido resolver un problema por divide vencerás, disponemos de amplio margen de maniobra para nuestra creativi-dad. Estudiaremos ahora dos de ellos —ordenar por fusión (mergesort) y ordenación rápida.

### Ordenación por fusión

El enfoque evidente de divide y vencerás para este problema consiste en descomponer la matriz T en dos partes cuyos tamaños sean tan parecidos como sea posible, ordenar estas partes mediante llamadas recursivas, y después fusionar las soluciones de cada parte, teniendo buen cuidado en mantener el or-den. Para hacer esto, necesitamos un algoritmo eficiente para fusionar dos matrices ordenadas U y V en una única matriz T cuya longitud sea la suma de las longitudes de U y V. Esto se puede lograr de forma más eficiente —y más sen-cilla— si se dispone de espacio adicional al final de las matrices U y V, para utilizarlo como centinela. (Esta técnica sólo funciona si podemos dar al centinela un valor previamente acordado y que estemos seguros que es mayor que cualquier elemento de U y V.

### Ordenación rápida (Quicksort)

A diferencia de ordenar por fusión, la mayor parte del trabajo no recursivo que hay que hacer se invierte en construir los subcasos, y no en combinar sus soluciones. Como primer paso, el algoritmo selecciona como pivote uno de los elementos de la matriz que haya que ordenar. A continuación, la matriz se parte a ambos lados del pivote: se desplazan los elementos de tal manera que los que sean mayores que el pivote queden a su derecha, mientras que los demás quedan a su izquierda. Si ahora las partes de la matriz que quedan a ambos lados del pivote se ordenan independientemente mediante llamadas recursivas al algoritmo, el resultado final es una matriz completamente ordenada; no hace falta un paso subsiguiente de fusión. Para equilibrar los tamaños de los dos subcasos que hay que ordenar, nos gustaría utilizar el elemento mediana como pivote (para una definición de la mediana, véase la Sección 7.5). Desafortunadamente, encontrar de la mediana requiere un tiempo excesivo. Por esta razón, nos limitamos a utilizar como pivote un elemento arbitrario de la matriz, y esperamos tener suerte.
El diseño de un algoritmo de partición con tiempo lineal no es tarea difícil. Sin embargo, en la práctica resulta crucial que la constante oculta sea pequeña, para que quicksort sea competitivo con otras técnicas de ordenación tales como ordenación por montículo. Supongamos que es preciso descomponer la submatriz I[i] empleando como pivote p = T[i].

## BÚSQUEDA DE LA MEDIANA

¿Qué podría ser más sencillo que buscar el menor elemento de T, o calcular la media de todos los elementos? Sin embargo, no es evidente que sea posible calcular la mediana con tanta facilidad. Un algoritmo sencillo para determinar la mediana de T[1..»] consiste en ordenar la matriz y extraer entonces el elemento In / 21- ésimo. Si utilizamos ordenación por montículo u ordenación por fusión, esto requiere un tiempo que está en ©( log n). ¿Podemos hacerlo mejor? Para responder a esta pregunta, estudiaremos la interrelación entre hallar la mediana y seleccionar el s-ésimo elemento más pequeño.
Es evidente que todo algoritmo para el problema de selección se puede utilizar para hallar la mediana: basta con seleccionar el [n / 27-ésimo elemento más pequeño. Curiosamente, la inversa también es cierta. Supongamos por el momento que está disponible un algoritmo mediano(T(1....]) que devuelve la mediana de T. Dada una matriz T y un entero s, ¿cómo se podría utilizar este algoritmo para determinar el s-ésimo elemento más pequeño de T? Sea p la mediana de
T. Ahora usamos p como pivote, de forma muy parecida a quicksort, pero usando el algoritmo pivotebis presentado al final de la sección anterior. Recuerde que una llamada a pivotebis(T[1.wl, p; var k, I) particiona a T[i..j] en tres secciones: T se reorganiza de tal manera que los elementos de T[i..k] sean más pequeños que p, los de T1k+1..I-1| sean iguales a p, y los de T[!..jl sean mayores que p. Tras una llamada a pivotebis(T, p, k, I), hemos terminado si k < s < I, puesto que entonces el s-ésimo elemento más pequeño de T es igual a p. Si s ≤ k, entonces el s-ésimo elemento más pequeño de T es ahora el s-ésimo elemento más pequeño de T[1..k].
Por último, si s ≥ l, entonces el s-ésimo elemento más pequeño de T es ahora el
(s - 1 + 1)-ésimo elemento más pequeño de Tl...]. En cualquier caso, hemos avanzado, porque o bien hemos terminado, o bien la submatriz que hay que considerar contiene menos de la mitad de los elementos, por cuanto p es la mediana de la matriz original.

## MULTIPLICACIÓN DE MATRICES

Siguiendo el descubrimiento de Strassen, un cierto número de investigadores ha intentado mejorar la constante a de tal manera que sea posible multiplicar dos matrices i X il en un tiempo que esté en O(°). Lo primero que se podía intentar, evidentemente, era multiplicar dos matrices 2 x 2 empleando seis multiplicaciones escalares. Pero en 1971, Hopcroft y Kerr demostraron que esto era imposible cuando no se puede emplear la conmutatividad de la multiplicación. Lo siguiente que había que intentar era encontrar una forma de multiplicar dos matrices 3 X 3 empleando como máximo 21 multiplicaciones escalares. Esto daría lugar a un algoritmo recursiva para multiplicar matrices i X il en un tiempo que estaría en O(nlog: 21), que es asintóticamente más rápido que el algoritmo de Strassen, porque log, 21 < log, 7. Desafortunadamente, esto también es imposible.
Pasó casi una década antes de que Pan descubriera una forma de multiplicar dos matrices 70 x 70 empleando 143.640 multiplicaciones escalares — comparese esto con las 343.000 que requiere el algoritmo clásico— y de hecho loga, 143.640 es un poquitín más pequeño que lg 7. Este descubrimiento dio pie a la denominada guerra de los decinales. Se fueron descubriendo sucesivamente numerosos algoritmos cada vez más eficientes asintóticamente. Por ejemplo, al final de 1979 se sabía que era posible multiplicar matrices en un tiempo que estaba en O(12521x)); imagine la excitación reinante en enero de 1980 cuando esto se mejoró hasta alcanzar O(12521801). El algoritmo de multiplicación matricial asintóticamente más rápido conocido en el momento de escribir esto se remonta a 1986, año en que Coppersmith y Winograd descubrieron que es posible, al menos en teoría, multiplicar dos matrices i X il en un tiempo que está en O(1237*).

## EXPONENCIACTÓN

Si deseamos manejar operandos más grandes, es preciso tener en cuenta el tiempo necesario para cada multiplicación. Sea M(v), s) el tiempo necesario para multiplicar dos enteros de tamaños q y s. Para nuestros propósitos, no in-porta si consideramos el tamaño de los enteros en dígitos decimales, en bits o en cualquier otra base fija mayor que 1. Supongamos por sencillez que 4, ≤ q2! s, ≤s, implican que M(gps) ≤ M(qp5,). Estimemos cuánto tiempo invierte nuestro algoritmo multiplicando enteros cuando se invoca exposec(a, i1). Sea m el tamaño de a. En primer lugar, observemos que el producto de dos enteros de tamaños i y j tiene un tamaño que es al menos i + j - 1 y como máximo i + j; véase el problema 7.24. Sean r, y m, el valor y el tamaño de r al principio de la i-ésima pasada por el bucle. Claramente, r, = a y por tanto m, = m. Dado que Ti= ar,, el tamaño de r, es al menos m + m, - 1 y como máximo m + m. La demostración por inducción matemática de que im - i + 1 Si, ≤ im para todo i se sigue inmediatamente. Por tanto, la multiplicación efectuada en la i-ésima pasada por el bucle afecta a un entero de tamaño m y a un entero cuyo tamaño se encuentra entre im - i + 1 e im, lo cual requiere un tiempo que está entre
Mon, im - i + 1) y M(m, im).

## ENSAMBLANDO TODAS LA PIEZAS: INTRODUCCIÓN A LA CRIPTOGRAFÍA

Retrotrayéndonos a la sección anterior, resulta descorazonador que una reducción exponencial del número de multiplicaciones necesario para calcular a" no se traduzca en un espectacular ahorro de tiempo de ejecución. Sin embargo, existen aplicaciones para las cuales es razonable contar todas las multiplicaciones como de un mismo coste. Tal es el caso si estamos interesados en la aritmética modular, esto es, en el cálculo de a" módulo algún tercer entero z. Recuerde que x mod z denota el resto de la división entera de x por z. Por ejemplo, 25 mod 7 = 4 porque 25
= 3X7 + 4. Si x e y son dos enteros entre 0 y z- I, v si z es un entero de tamaño m, entonces la multiplicación modular xy mod z necesita una multiplicación entera ordinaria de dos enteros de tamaño in como máximo, dando lugar a un entero de tamaño 2m como máximo, seguida por división del producto por z, un entero de tamaño m, para calcular el resto de la división. Por tanto, el tiempo que requiere cada multiplicación.

## PROGRAMACIÓN DINÁMICA Semana 8
## DOS EJEMPLOS SENCILLOS
### Cálculo del coeficiente binomial
### El campeonato mundial
## DEVOLVER CAMBIO (2)
## EL PRINCIPIO DE OPTIMALIDAD
## EL PROBLEMA DE LA MOCHILA (2)
## CAMINOS MÍNIMOS
## MULTIPLICACIÓN ENCADENADA DE MATRICES
## ENFOQUES QUE APLICAN RECURSIÓN
## FUNCIONES CON MEMORIA

# Talleres 

![image](https://github.com/user-attachments/assets/90e2ac91-9a83-4bc7-ba8d-e2d795b7ef00)
Proceso de Insertar 
```
para i ← 2 hasta n hacer
    x ← T[i]; j ← i - 1
    mientras j > 0 y x < T[j] hacer
        T[j + 1] ← T[j]
        j ← j - 1
    T[j + 1] ← x
```
Proceso de Seleccionar 
```
para i ← 1 hasta n - 1 hacer
    minj ← i; minx ← T[i]
    para j ← i + 1 hasta n hacer
        si T[j] < minx entonces
            minj ← j
            minx ← T[j]
    T[minj] ← T[i]
    T[i] ← minx
```
![image](https://github.com/user-attachments/assets/3aad2066-f822-48ef-bd4c-0c807249a16c)
![image](https://github.com/user-attachments/assets/4126e990-80d5-4b37-b364-eca6df1f149e)
![image](https://github.com/user-attachments/assets/88da33bd-bf51-428b-971c-5286b376ca09)
![image](https://github.com/user-attachments/assets/da8674ce-a6d6-4110-9d75-f06627fde032)
![image](https://github.com/user-attachments/assets/63592516-de95-4e9a-83a1-a2503a20f581)

## Taller de pasarlo a java 
public class MergeSort {

    public static void mergeSort(int[] A, int p, int r) {
        if (p < r) {
            int q = (p + r) / 2;
            mergeSort(A, p, q);
            mergeSort(A, q + 1, r);
            merge(A, p, q, r);
        }
    }

    public static void merge(int[] A, int p, int q, int r) {
        int nL = q - p + 1;
        int nR = r - q;

        int[] L = new int[nL];
        int[] R = new int[nR];

        for (int i = 0; i < nL; i++) {
            L[i] = A[p + i];
        }

        for (int j = 0; j < nR; j++) {
            R[j] = A[q + 1 + j];
        }

        int i = 0, j = 0, k = p;

        while (i < nL && j < nR) {
            if (L[i] <= R[j]) {
                A[k++] = L[i++];
            } else {
                A[k++] = R[j++];
            }
        }

        while (i < nL) {
            A[k++] = L[i++];
        }

        while (j < nR) {
            A[k++] = R[j++];
        }
    }

    // Método principal para probarlo
    public static void main(String[] args) {
        int[] A = {2, 5, 8, 3, 6, 7};
        mergeSort(A, 0, A.length - 1);

        // Imprimir el arreglo ordenado
        for (int num : A) {
            System.out.print(num + " ");
        }
    }
}
![image](https://github.com/user-attachments/assets/b242a124-0e28-4bf3-8c45-7c7d249fc16a)
![image](https://github.com/user-attachments/assets/0c99e59a-7302-4837-b6e7-72433bfdc642)
![image](https://github.com/user-attachments/assets/c76fdf1c-83ed-4acd-90df-6edbabd75a64)
```java
public class Solucion {
    public static void main(String[] args) {
        int resultado = calcularResultado(10); // Puedes ajustar el valor según sea necesario
        System.out.println("El resultado es: " + resultado);
    }

    public static int calcularResultado(int n) {
        if (n <= 1) {
            return 1;
        }
        return 2 * calcularResultado(n - 1) + 1;
    }
}
```
![image](https://github.com/user-attachments/assets/ed4397f8-8073-4cf8-869a-b4b9abd48721)
![image](https://github.com/user-attachments/assets/95135ac6-5881-4245-ad2c-5afd4e721b04)
![image](https://github.com/user-attachments/assets/a1d5d9ba-01a4-4ab1-93c4-e21130eec051)
![image](https://github.com/user-attachments/assets/63fe586a-a397-42f5-9291-54ee043c7c25)

![image](https://github.com/user-attachments/assets/d79845db-8704-4c50-b642-9bbf13a433a7)




