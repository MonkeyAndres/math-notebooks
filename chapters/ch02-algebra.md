# Algebra

## Polinomios

Un monómio es un producto de números reales e indeterminadas. Llamamos coeficiente a la parte real y parte literal a la indeterminada.

Un polinomio es un conjunto de monómios y su grado es igual al del monómio de mayor grado

### Operaciones con polinomios

- Suma: suma los monomios con la misma parte literal
- Resta: resta los monomios con la misma parte literal
- Producto: multiplicación de coeficientes y suma de exponentes en parte literal
- División: aplicando el algoritmo normal de las divisiones. [Explicación](https://youtu.be/9SOVM5WN0eI)

Propiedades de los polinomios

- Conmutativa: el orden no afecta al resultado
- Asociativa: se puede agrupar una suma o resta de tres o mas polinomios de cualquier manera obteniendo siempre el mismo resultado
- Elemento neutro
- Elemento opuesto: el opuesto de un polinomio sumado al polinomio inicial resulta en el elemento neutro
- Distributiva: $p(q+r) = (p*q) + (p*r)$

### Prodúctos notables

- $(a+b)^2 = a^2 + 2ab + b^2$
- $(a-b)^2 = a^2 - 2ab + b^2$
- $(a+b)^3 = a^3 + 3a^2b + 3ab^2 + b^3$
- $(a-b)^3 = a^3 - 3a^2b + 3ab^2 - b^3$
- $(a+b)(a-b) = a^2 - b^2$

### Regla de Ruffini

Es un algoritmo que nos proporciona una manera mas facil de dividir polinomios siempre y cuando e l divisor tenga la forma $x-a$. [Explicación de Ruffini](https://youtu.be/nuapNH8T9gQ)

### Teorema del resto

Al dividir un polinomio $P(x)$ entre $(x - a)$ el resto es igual a $P(-a)$. Es muy util para hallar los valores numericos de polinomios sin necesidad de sustituir directamente la incognita.

### Raices de un polinomio

El teorema del resto nos permite saber si un numero es raiz de un polinomio. Simplemente cogemos el numero que tenemos que comprobar, por ejemplo $a$ y comprobamos que $P(a) = 0$.

Para hallar las raices enteras de un polinomio:

- Se calculan divisores del termino independiente del polinomio
- Se prueban todos sus divisores y los que cumplan con el teorema del resto o con Ruffini son raices

Por ejemplo: Las raices enteras de $x^3 + 2x^2 + x -6$ estan entre $\pm 1, \pm2, \pm 3, \pm 6$ pero solo son $2, -3$

Para hallar las raices racionales de un polinomio:

- Se calculan divisores del termino independiente del polinomio
- A cada divisor le ponemos como denominador el coeficiente del termino de mayor grado
- Se prueban todos sus divisores y los que cumplan con el teorema del resto o con Ruffini son raices

Por ejemplo: Las raices racionales de $2x^3 + 2x^2 + x -6$ estan entre $\frac {\pm 1} 2, \frac {\pm 2} 2, \frac {\pm 3} 2, \frac {\pm 6} 2$ pero solo es$\frac {-1} 2$

### Factorización de polinomios

Un polinomio es divisible por $(x-a)$ siempre y cuando $a$ sea una raiz de ese polinomio. Basandonos en este enunciado podemos reducir un polinomio siempre y cuando este tenga raices y repetir este proceso hasta que obtengamos un polinomio sin raices ergo irreducible.

Para reducir un polinomio simplemente aplicamos Ruffini con un numero raiz del polinomio, nos quedamos el coeficiente y reescribimos el polinomio como $P(x) = c(x) * (x-a)$

### Fracciones algebraicas

Son expreciones en las que numerador y denominador son polinomios y el polinomio denominador es distinto de 0. Para simplificarlas simplemente de pueden factorizar ambos terminos y reducir como se hace con las fracciones formales.

### Operaciones con fracciones algebraicas

- Suma o resta: hay que conseguir mismo denominador (factorizando denominador y sacando factor comun) y despues se suman o restan los numeradores
- Producto: multiplicar los numeradores y denominadores
- Division: regla de la divison de fracciones numericas $\frac {\frac {p1} {q1}} {\frac {p2} {q2}} = \frac {p1 * q2} {q1 * p2}$

## Ecuaciones

### Resolver ecuaciones de primer grado

1. Suprimir denominadores: multiplicar numeradores por el MCM de los denominadores
2. Efectuar parentesis
3. Transponer terminos y simplificar
4. Despejar la incógnita y simplificar resultado
5. Comprobar resultado

### Resolver ecuaciones de segundo grado

Tienen la forma $ax^2+bx+c=0$

Las ecuaciones de segundo grado pueden tener 2, 1 o ninguna solucion en el campo real.

- Caso 1 ($b= 0$) simplemente despejar la $x$
- Caso 2 ($c = 0$) sacar factor comun y despejar $x$. Siempre una solucion es 0
- Caso 3 (completo): $x = \frac {-b \pm \sqrt {b^2-4ac}} {2a}$

La representacion grafica de una ecuacion de segundo grado depende de el signo del coeficiente de $x^2$, si es positivo la funcion tendra forma de U y si es negativo tendra forma de $\cap$. Por otro lado las soluciones de la ecuacion seran los puntos de corte de esa ecuacion con el eje de abscisas.

### Sacar la ecuacion de segundo grado de sus soluciones

Suma y producto de soluciones de ecuacion de segundo grado nos dan estas dos igualdades al reducir ($x1$ primera solucion de la ecuacion y $x2$ segunda solucion de la ecuacion):

- $x1 + x2 = \frac {-b} a$
- $x1 * x2 = \frac c a$
- $ax^2+bx+c=0$ es lo mismo que $x^2 + \frac b a x+ \frac c a = 0$

Teniendo en mente estas igualdades podemos resolver el problema inverso, teniendo las soluciones de una ecuacion de segundo grado podemos saber la ecuacion de la que son solucion. La tercera igualdad se puede relacionar con las otras dos y reeplazar como $x^2-(x1 + x2)x + x1 * x2 = 0$

Ejemplo: Soluciones $x1 = 1/2$ y $x2 = 2/3$

1. $x^2-(\frac 1 2 + \frac 2 3)x + \frac 1 2 * \frac 2 3 = 0$
2. $x^2-\frac 7 6 + \frac 2 6 = 0$
3. $6x^2-7x+2=0$

### Ecuaciones bicuadradas

Las ecuaciones bicuadradas tienen esta pinta $ax^4+bx^2+c = 0$. Para resolverlas simplemente hacemos un cambio de variable $x^2 = t$ y transformamos la ecuacion en $at^2+bt+c=0$ que es una ecuacion de segundo grado facil de resolver. Una vez halladas sus soluciones deshacemos el  cambio de variable $x = \pm \sqrt t$

## Inecuaciones

Una incecuacion es una desigualdad algebraica en la que aparecen una o mas incognitas. Su grado se determina por el mayor de los grados al que este elevado sus incognitas.

Resolver la ecuacion consiste en encontrar los valores que la verifican

### Inecuaciones equivalentes

Parte del trabajo de resolver inecuaciones se simplifica cuando se encuentra otra equivalente mas sencilla. Para esto se pueden aplicar estas transformaciones:

- Sumar o restar la misma expresion a los dos miembros
- Multiplicar o dividir ambos miembros por un numero positivo
- Multiplicar o dividir por un numero negativo y cambiar la orientacion del signo (de < a > y viceversa)

### Resolucion de inecuaciones de primer grado

Se resuelven exactamente igual que las ecuaciones de primer grado solo que su solucion es un conjunto. ([Repasar conjuntos]())

OJO: al pasar un numero negativo de lado hay que cambiar la orientacion del signo

Dependiendo de la orientacion del signo de la inecuacion debemos definir el conjunto como:

- $x < 0 = (-\infin, 0)$
- $x > 0 = (0, +\infin)$
- $x \leq 0 = (-\infin, 0]$
- $x \geq 0 = [0, +\infin)$

Siendo el $0$ el valor tras despejar la $x$ de la inecuacion

### Resolucion de inecuaciones de segundo grado

Se resuelven igual que las ecuaciones de segundo grado pero una vez obtenidos sus resultados hay que averiguar en conjunto solucion de este intervalo. Para ello planteamos 3 entornos (siendo $x1$ la solucion mas proxima a $-\infin$ y $x2$ la mas proxima a $+\infin$:

- $(-\infin, x1)$
- $(x1, x2)$
- $(x2, +\infin)$

Escogemos un valor dentro de cada entorno y sustituimos ese valor de $x$ en la inecuacion simplificada (con el 0 a un lado). Anotamos si la solucion da positivo o negativo y en base a la ecuacion cogemos el conjunto que la resuelve.

[Video explicando esto mucho mas chachi.](https://youtu.be/AZ1_gwZSi-g)

## Sistemas de ecuaciones lineales

Los sistemas de ecuaciones son ecuaciones en las que todas sus incógnitas están elevadas a la unidad, no pudiendo aparecer el producto de dos de ellas.

Dependiendo del tipo de solución se clasifican en:

- Compatible: tienen solución
  - Determinado: solución única, rectas secantes
  - Indeterminado: infinitas soluciones, rectas paralelas
- Incompatible: no tiene solución

### Métodos para resolver sistemas de ecuaciones lineales

- Sustitución: despejar cualquier incógnita y sustituir el valor en otra ecuación

- Igualación: despejar una incógnita en todas las ecuaciones e igualar los valores

- Reducción: consiste en intentar eliminar una de las incógnitas transformando las ecuaciones del sistema en ecuaciones equivalentes y tratándolas como una suma

  Ej: $\begin{cases} 4x + y = -3 \\ -3x + y = 11 \end{cases} \Harr \begin{cases} 4x + y = -3 \\ 3x - y = -11 \end{cases} \Harr 7x = -14 \Harr x = -\frac {14} 7 \Harr x = -2$ 

- Método de Gauss: se puede aplicar a cualquier numero de ecuaciones e incógnitas y consiste en dejar la ultima ecuación con 1 incógnita, la penúltima con 2 y así siguiendo hacia arriba.

  Para conseguir esto usamos el método de reducción con la ultima y la penúltima ecuación hasta dejar la ultima con 1 incógnita (resultado de reducción de ultima y penúltima) y luego pasamos a la penúltima y dejamos 2 incógnitas y así hasta acabar en la ultima ecuación.

  Una vez reducida la ultima ecuación nos dará el valor de una incógnita y al sustituir en la penúltima nos dará otra incógnita y así sucesivamente hasta resolver todo el sistema

  [Video explicando esto.](https://youtu.be/Ix9hDqfNuIA)

### Sistemas de inecuaciones lineales

[Sistemas de inecuaciones lineales una y dos incognitas.mp4](https://youtu.be/42ZjyjG7HG0)