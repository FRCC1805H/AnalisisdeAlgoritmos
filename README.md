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

### Bucles "para" (desde).
### Llamadas recursivas
### Bucles "mientras" y "repetir"
## USO DE UN BARÓMETRO
## ANÁLISIS DEL CASO MEDIO
## ANÁLISIS AMORTIZADO
## RESOLLCIÓN DE RECURRENCIAS
### Suposiciones inteligentes
### Recurrencias homogéneas
### Recurrencias no homogéneas
### Cambios de variable
### Transformaciones de intervalo
### Recurrencias asintóticas.

## ESTRUCTURAS DE DATOS Semana 5
## MATRICES (ARRAYS), PILAS Y COLAS
## REGISTROS Y PUNTEROS (APUNTADORES)
## LISTAS
## GRAFOS
## ÁRBOLES
## TABLAS ASOCIATIVAS
## MONTÍCULOS (HEAPS) 
## MONTÍCULOS BINOMIALES
## ESTRUCTURAS DE CONJUNTOS DISJUNTOS (PARTICIÓN)

## ALGORIIMOS VORACES Semana 6
### DAR LA VUELTA (1) 
### CARACTERÍSTICAS GENERALES DE LOS ALGORITMOS VORACES
### GRAFOS: ÁRBOLES DE RECUBRIMIENTO MÍNIMO
### Algoritmo de Kruskal
### Algoritmo de Prim
## GRAFOS: CAMINOS MÍNIMOS
## EL PROBLEMA DE LA MOCHILA (I)
## PLANIFICACIÓN 
### Minimización del tiempo del sistema
### Planificación con plazo fijo

## DIVIDE Y VENCERÁS Semana 7
## INTRODUCCIÓN: MULTIPLICACIÓN DE ENTEROS MUY GRANDES
## EL CASO GENERAL
## BÚSQUEDA BINARIA
## ORDENACIÓN 
### Ordenación por fusión
### Ordenación rápida (Quicksort)
## BÚSQUEDA DE LA MEDIANA
## MULTIPLICACIÓN DE MATRICES
## EXPONENCIACTÓN
## ENSAMBLANDO TODAS LA PIEZAS: INTRODUCCIÓN A LA CRIPTOGRAFÍA

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

## Taller de pasarlo a java 
public class MergeSort {

    // Función que combina dos subarreglos ordenados
    public static void merge(int[] A, int p, int q, int r) {
        int nL = q - p + 1; // Tamaño del subarreglo izquierdo
        int nR = r - q;     // Tamaño del subarreglo derecho

        // Crear arreglos temporales
        int[] L = new int[nL];
        int[] R = new int[nR];

        // Copiar los datos a los arreglos temporales
        for (int i = 0; i < nL; i++) {
            L[i] = A[p + i];
        }

        for (int j = 0; j < nR; j++) {
            R[j] = A[q + 1 + j];
        }

        int i = 0, j = 0, k = p;

        // Mezclar los arreglos temporales de vuelta al arreglo original A
        while (i < nL && j < nR) {
            if (L[i] <= R[j]) {
                A[k] = L[i];
                i++;
            } else {
                A[k] = R[j];
                j++;
            }
            k++;
        }

        // Copiar los elementos restantes de L, si hay alguno
        while (i < nL) {
            A[k] = L[i];
            i++;
            k++;
        }

        // Copiar los elementos restantes de R, si hay alguno
        while (j < nR) {
            A[k] = R[j];
            j++;
            k++;
        }
    }

    // Función recursiva Merge Sort
    public static void mergeSort(int[] A, int p, int r) {
        if (p < r) {
            int q = (p + r) / 2;
            mergeSort(A, p, q);
            mergeSort(A, q + 1, r);
            merge(A, p, q, r);
        }
    }

    // Función para imprimir un arreglo
    public static void printArray(int[] A) {
        for (int i : A) {
            System.out.print(i + " ");
        }
        System.out.println();
    }

    // Método principal para probar Merge Sort
    public static void main(String[] args) {
        int[] arr = {38, 27, 43, 3, 9, 82, 10};
        System.out.println("Arreglo original:");
        printArray(arr);

        mergeSort(arr, 0, arr.length - 1);

        System.out.println("Arreglo ordenado:");
        printArray(arr);
    }
}


