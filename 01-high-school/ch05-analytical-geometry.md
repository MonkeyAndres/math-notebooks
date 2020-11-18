# Geometría Analítica

## Vectores

Un vector $\vec{v}(2,3)$ representa un movimiento del plano mientras que un punto $P(1,-2)$ representa una posición en el plano. Los vectores se suelen denotar con letras minúsculas y flechas encima $\vec{v}$

- Magnitudes vectoriales: se describen con un vector
- Magnitudes escalares: se describen con un numero
- Escalar: numero (se le llama asi para distinguir de vectores)

### Características de un vector

- Modulo: representa el tamaño del vector, es decir, la distancia que se recorre al aplicar el vector. Se calcula así $||\vec{v}|| = \sqrt {v_1^2 + v_2^2}$. Se dice que es unitario si tiene modulo 1
- Dirección: pendiente de la recta que contiene el vector, se calcula como $m = v_2/v_1$. Dos vectores con la misma direccion son paralelos
- Sentido: indicado por la punta de la flecha

En Física se distingue entre vectores libres (que representan un desplazamiento) y vectores ligados (que están asociados a un punto). Pero en matemáticas se suelen usar vectores libres.

### Operaciones con puntos y vectores

- Vector que une dos puntos $\vec{PQ} = {(q_1 - p_1, q_2-p_2)}$
- Suma punto + vector $(p_1 + v_1, p_2 + v_2)$
- Suma dos vectores $(v_1 + w_1, v_2 + w_2)$
- Producto vector y escalar $(k*v_1, k*v_2)$
- Distancia entre dos puntos $||\overrightarrow{PQ}||$
- Hallar el vector unitario: $\vec{v} \over |\vec{v}|$

### Producto escalar

Se calcula como $\vec{v} * \vec{w} = v_1 * w_1 + v_2 * w_2$

Propiedades:

- Conmutativa: $\vec{v} * \vec{w} = \vec{w} *\vec{v}$
- Distributiva respecto a suma: $\vec{v}*(\vec{u} + \vec{w}) = \vec{v} * \vec{u} + \vec{v} * \vec{w}$
- Asociativa respecto a escalares (siendo $k$ escalar): $\vec{v} * (k\vec{w}) = (k\vec{v}) * \vec{w} = k(\vec{v}*\vec{w})$
- El producto escalar es el producto de módulos por el coseno del ángulo que forman (siendo $\alpha$ el ángulo que forman): $\vec{v} * \vec{w} = ||\vec{v}|| *  ||\vec{w}|| * cos(\alpha)$

El producto escalar se usa para el calculo de los ángulos tal que $cos(\alpha) = {\vec{v} * \vec{w} \over ||\vec{v}|| * ||\vec{w}||}$

### Bases ortogonales

Un vector es perpendicular a otro si su producto escalar es igual a $0$. Para calcular un vector perpendicular a otro simplemente hay que hacer $\vec{v} = (v_1,v_2) \rarr \vec{w} = (-v_2, v_1)$

Para comprobar si dos vectores forman base ortogonal tenemos que comprobar:

- Que sean perpendiculares
- Que sean linearmente independientes ⇒ ${v_1 \over v_2} \not = {w_1 \over w_2}$

### Bases ortonormales

Para comprobar si dos vectores forman base ortogonal tenemos que comprobar:

- Que formen base ortogonal
- Que ambos vectores sean unitarios

## Rectas y problemas metricos

Un lugar geométrico son los puntos del plano que verifican una o varias condiciones geométricas

Una recta es un lugar geométrico de los puntos del plano que se pueden alcanzar sumando a un punto múltiplos de un vector (vector director). Resumiendo si cogemos un punto y le vamos sumando múltiplos del vector obtenemos infinitos puntos de la recta.

### Ecuación vectorial y paramétrica

Dado un punto $P=(p_1, p_2)$ y un vector director $\vec{v} = (v_1, v_2)$:

- Se llama ecuación vectorial a la expresión de $\{ (x,y)=(p_1, p_2) + k*(v_1, v_2) \}$
- Se llama ecuación paramétrica a la expresión $\begin{cases}
  x = p_1 + v_1*k \\
  y = p_2 + v_2*k
  \end{cases}$

Se habla de un vector director ya que todos los vectores paralelos a un vector director son también directores

La ecuación vectorial y paramétrica (que son iguales) son muy útiles para calcular puntos de la recta

### Ecuación continua

Es una ecuación que nos sirve para comprobar si un punto pertenece a una recta o no. 

Para calcular al ecuación partimos de la ecuación paramétrica y ya que buscamos una ecuación que relacione la $x$ con la $y$, para ello despejamos la $k$ a un lado de la ecuación e igualamos y nos queda: ${x-p_1 \over v_1} = {y-p_2 \over v_2}$

Para comprobar si un punto pertenece a la recta sustituimos los valores de la recta en la ecuación (vector director y punto) y sustituimos $(x, y)$ por los valores del punto a comprobar. Si se cumple la igualdad pertenece, sino no

### Ecuación punto-pendiente

El problema con las ecuaciones anteriores es que para cada punto-vector nos sale una ecuación diferente lo cual hace difícil identificar si hablamos de la misma recta.

Para ello teniendo en cuenta que la pendiente de una recta es la pendiente de un vector director suyo podemos expresar una recta como $y-p_2 = m(x-p_1)$

Esta expresión no es única ya que depende del punto pero al menos no depende del vector

Ahora para calcular si un punto pertenece a una recta solo tenemos que tener la pendiente, y un punto, sustituimos la $x$ o la $y$ y si el resultado da la otra cordenada del punto el punto pertenece

### Ecuación implícita o general

Otro modo de expresar una ecuación lineal tiene forma $Ax + By + C = 0$

Donde $A = v_2, B = -v_1, C = v_1p_2 - v_2p_1$

Teniendo una recta en esta forma podemos calcular el vector director como $\overrightarrow{(-B, A)}$

### Ecuación explicita

Es una ecuación que siempre es única se puede calcular a partir de la ecuación punto pendiente despejando la $y$

Queda una ecuacion $y = mx +n$ donde $m$ es la pendiente de la recta y $n$ es el punto de corte con el eje $y$ cuando $x = 0$

### Posiciones relativas de rectas

Desde el punto de vista geométrico, las posiciones de dos rectas en el plano son:

- Secantes: un punto en común
- Paralelas: ningún punto en común y misma pendiente
- Coincidentes: misma recta

Para distinguir que posición ocupan dos rectas tenemos dos métodos

- Con vectores directores
  1. Calcular los vectores directores de las dos rectas. Si NO son paralelos, son secantes.
  2. Si los vectores son paralelos, tomar un punto cualquiera de una recta y ver si es punto de la otra. Si lo es, son coincidentes. Si no, son paralelas.
- Analizar y resolver sistema. Pasar ambas rectas a forma general y ponerlas en forma de sistema. El sistema puede ser:
  - Compatible determinado (secantes): ${A_1 \over A_2} \not = {B_1 \over B_2}$
  - Compatible indeterminado (coincidentes): ${A_1 \over A_2} = {B_1 \over B_2} = {C_1 \over C_2}$
  - Incompatible (paralelas): ${A_1 \over A_2} = {B_1 \over B_2} \not = {C_1 \over C_2}$
- Resolver sistema. Pasar ambas rectas a forma general y ponerlas en forma de sistema y resolver
  - Si sale un punto → Secantes
  - Si sale $0=0$ → Coincidentes
  - Si sale $1 = 0$ → Paralelas

### Distancia de un punto a una recta

La distancia entre un punto y una recta es la mínima distancia que hay entre un punto y cualquiera de los puntos de la recta.

Pasos dado un punto $P$  y una recta $r$:

1. Calcular la recta perpendicular a $r$ calculando el vector perpendicular y haciendo que pase por el punto $P$. Usar forma continua que es mas fácil.
2. Convertir $r$ en ecuación continua (para que tenga $x$ e $y$)
3. Poner ambas ecuaciones de la recta en un sistema y resolver el sistema. Esto nos dará el punto de corte con la recta $r$
4. Teniendo este punto de corte hay que calcular la distancia entre el punto $P$ y el punto de corte

Formula general distancia de un punto a recta (no distancia minima): $d(P,r) = |{Ax+By+C \over \sqrt {A^2+B^2}}|$

### Punto simétrico

Dada una recta y un punto exterior a ella es un punto situado a la misma distancia de la recta pero en el otro lado de la recta. Ambos puntos deben estar en la misma recta (el simétrico y el dado).

Formula: $P' = Q + \overrightarrow{PQ}$ siendo $Q$ el punto de $r$ de mínima distancia a $P$

### Traslaciones de rectas

Si queremos transformar el punto $(x_0,y_0)$ en el origen de coordenadas se hace $\begin{cases}
x' = x-x_0 \\
y' = y - y_0
\end{cases}$

modo la nueva ecuación aparece centrada en el origen.

Ejemplo: trasladar la recta $2y + x = 3$ para que pase por el punto $(0,0)$

1. Pasar todo a un lado de la igualdad

   $2y + x -3 = 0$

2. Agrupar el termino independiente con la $x$ o la $y$

   $2y + (x-3) = 0$

3. Sustituir según la igualdad de arriba

   $2y+x=0$

4. Listo, esta nueva recta ya pasa por el punto $(0,0)$

Ejemplo: trasladar la recta $2y + x = 3$ para que pase por el punto $(-2,-1)$

1. Pasar todo a un lado de la igualdad

   $2y + x -3 = 0$

2. Sustituir la $(x-3) \rarr x-(-2); y\rarr y-(-1)$

   $2(y+1) + (x+2) = 0$

3. Resolver

   $2y+2+x+2=0\rarr 2y+x+4=0$

4. Listo, esta nueva recta ya pasa por el punto  $(-2,-1)$

Ejemplo: calcular la recta con pendiente 2 que pase por el punto $(-1,2)$

1. Escribir la recta que pasa por $(0,0)$

   $y=2x$

2. Sustituir la $x \rarr x-(-1); y\rarr y-2$

   $(y-2)=2(x+1)$

3. Resolver y listo

   $y = 2x+4$

PARA COMPROBAR TRANSLACIONES: [https://www.geogebra.org/graphing?lang=es](https://www.geogebra.org/graphing?lang=es)

### Mediatriz

La mediatriz de un segmento $AB$ es un punto que esta en medio de ambos extremos del segmento, ergo que $d(X, A) = d(X,B)$

Tiene una formula general pero es inútil memorizarla, para calcular la mediatriz te pueden pedir:

Hallar el punto medio del segmento simplemente hacemos $M = {A+B \over 2}$

Hallar la recta que corta el segmento en 2:

1. Iguala la ecuación de la distancia de ambos puntos
2. Eleva el cuadrado ambos términos para quitarte la raíz cuadrada
3. Resuelve y te quedara la ecuación de una recta perpendicular al segmento que lo corta por la mitad

### Bisectriz

La bisectriz de dos rectas son otras dos rectas que cortan las rectas justo por la mitad.

Dadas las rectas $r$ y $s$ su bisectriz o bisectrices son $d(X, r) = d(X,s)$. Esto nos puede dar 1 o 2 soluciones dependiendo de las rectas. Simplemente resolvemos y ya. [Video explicación.](https://www.youtube.com/watch?v=RYgTv-IYi94)

## Cónicas

Existen 4 cónicas las cuales son

- Circunferencias
- Elipses
- Hipérbolas
- Parabolas

Todas comparten ciertas características y elementos (mirar cada apartado) entre ellos están que todas pueden ser representadas como ecuación general o ecuación canónica.

### Identificar cónicas

Para identificar de que cónica estamos hablando dada una ecuación general debemos fijarnos en ciertos factores.

Dada la ecuación general $Ax^2+By^2+Cx+Dy+E=0$

- Circunferencia: $A = B$ y mismo signo
- Elipse: $A$ y $B$ no son nulos y tienen el mismo signo.
- Hipérbola: $A$ y $B$ no son nulos y tienen distinto signo.
- Parábola
  - $A = 0; C \ne 0$
  - $B = 0; D \ne 0$

### Ecuación general - Ecuación canónica

Para pasar de una ecuación general a una canónica la clave es [completar cuadrados](http://www.disfrutalasmatematicas.com/algebra/completar-cuadrado.html) en vez de despejarlos.

Ejemplo: $9x^2-4y^2-18x-8y-31=0$

1. Agrupamos los términos con $x$ y los términos con $y$

   $9x^2-18x-4y^2-8y=31$

2. Sacamos factor común de los coeficientes cuadrados. El objetivo es dejar coeficiente $1$

   $9(x^2-2x)-4(y^2+2y)=31$

3. Completamos cuadrados

   $9(x^2-2x+1-1)-4(y^2+2y+1-1)=31$

   $9[(x-1)^2-1]-4[(y+1)^2-1]=31$

4. Pasamos términos sin incógnita a un lado

   $9(x-1)^2-4(y+1)^2=31+9-4$

   $9(x-1)^2-4(y+1)^2=36$

5. Para dejar un 1 a un lado de la ecuación tenemos en cuenta que $36 = 36*1$ ergo:

   ${9(x-1)^2 \over 36} - {4(y+1)^2 \over 36}=1$

6. Reducimos

   ${(x-1)^2 \over 4} - {(y+1)^2 \over 9}=1$

### Ecuación canónica - Ecuación general

Para pasar de una ecuacion canonica de cualquier figura conica a una ecuacion general lo unico que hay que hacer es despejar los cuadrados y reducir.

Ejemplo: ${(x-1)^2 \over 4}-{(y+1)^2 \over 9} = 1$

1. Despejamos cuadrados

   ${x^2-2x+1 \over 4} - {y^2 + 2y +1 \over 9} = 1$

2. Hacemos la resta de fracciones

   ${9(x^2-2x+1)-4(y^2+2y+1)\over 36} = 1$

3. Pasamos dividiendo y resolvemos

   $9x^2-18x+9-4y^2-8y-4=36$

4. Ordenamos

   $9x^2-4y^2-18x-8y-31=0$

### Circunferencias

Dado un punto $P$ cualquiera llamado centro y una distancia $r$ llamada radio, una circunferencia es el lugar geométrico de los puntos que están a distancia $r$  de $P$.

Para saber si un punto pertenece a una circunferencia tenemos que calcular $d[(x,y), (p_1,p_2)]=r$

Despejando obtenemos la ecuación canónica o reducida: $(x-p_1)^2+(y-p_2)^2=r^2$

#### Propiedades de las circunferencias

- Si se toman dos puntos de una circunferencia la mediatriz del segmento que los une pasa siempre por el centro
- Si tomamos un punto de una circunferencia la tangente a la circunferencia que pasa por ese punto es perpendicular al radio que le corresponde
- Conocidos tres puntos de la circunferencia podemos calcular la misma:
  1. Calcular las bisectrices de ambos segmentos ($AB$ y $BC$)
  2. Calcular el punto de corte entre ambas resolviendo el sistema resultante de las dos rectas. El resultado es el centro de la circunferencia
  3. El radio es la distancia desde el punto anterior y cualquiera de los 3 puntos

### La elipse

Una elipse es el lugar geométrico de los puntos cuya suma de distancias a dos puntos fijos (focos) es siempre constante. Dicho de otra forma $d(P, F_1) + d(P,F_2) = 2a$

Esa constante $2a$ sale de que la suma de la distancia entre los focos da como resultado una constante que coincide con la longitud del eje mayor.

Ecuación canónica (siendo $(h, k)$ el centro de la elipse): $({x-h\over a})^2+({y-k\over b})^2=1$.

#### Elementos de una elipse

TL;DR

Dada la ecuación canónica podemos sacar fácilmente los elementos de una elipse pero vamos a explicarlo poco a poco para que se entienda el porque.

![http://ares.cnice.mec.es/tecnologia/7/13/imagenes/67_e.gif](http://ares.cnice.mec.es/tecnologia/7/13/imagenes/67_e.gif)

---

- Los focos ya mencionados supongamos que son $F_1 , F_2$ dados estos focos podemos suponer que el centro de la elipse se encuentra en el medio de ellos dos.

  Vamos a suponer que la elipse esta centrada en el centro, para lo cual creamos una distancia arbitraria $c$ que seria la distancia entre el centro y los focos. Dicho esto nos queda que los focos estan en:

  $F_1 = (-c, 0); F_2 = (c, 0)$

  Esto cumple que ${F_1(-c, 0) + F_2(c, 0) \over 2} = (0, 0)$

- Distancia focal: $d(F_1, F_2) = 2c$

- Centro sabiendo focos: ${F_1 + F_2 \over 2}$

- El eje mayor como hemos visto es el resultado de $d(P, F_1) + d(P, F_2)$ esto lo podemos comprobar asumiendo que hay un punto $(a, 0)$ en la elipse y sustituyendo.

- Eje menor: Para calcular el eje menor podemos usar Pitágoras ya que $b^2 = a^2 - c^2$

- Excentricidad (es como el grado de ovalación): $e = c/a$

- Para saber cual es el eje mayor y cual el menor, comprobamos el dividendo mayor, este indica cual es el eje mayor y por lo tanto es $a$. Por ejemplo, teniendo $({x\over 10})^2+({y\over 20})^2=1$ podemos ver que el eje mayor es $y$ y $a = \sqrt{20}$ y por lo tanto $b = \sqrt{10}$

  Sabiendo esto sabemos que $a$ va con el eje mayor, $b$ con el eje menor y $c$ con el mayor

[Resumen muy bien explicado](https://www.aulafacil.com/cursos/matematicas/conicas/elipse-l10805)

### Hipérbolas

Una hipérbola es el lugar geométrico de los puntos cuya diferencia a unos puntos fijos (focos) en valor absoluto es constante. Dicho de otra forma $|d(P, F_1)-d(P,F_2)| = 2a$

Nuevamente esta constante resultante coincide con el eje mayor de la hipérbola, $2a$.

Ecuación canónica (siendo $(h, k)$ el centro de la hipérbola): $({x - h \over a})^2 -({y - k \over b})^2 = 1$

#### Elementos de una hipérbola

TL;DR

Dada la ecuación canónica podemos sacar fácilmente los elementos de una hipérbola pero vamos a explicarlo poco a poco para que se entienda el porque.

![](https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fimage.slidesharecdn.com%2Flasconicas-101023103503-phpapp01%2F95%2Flas-conicas-11-638.jpg%3Fcb%3D1422633563&f=1&nofb=1)

---

- En las hipérbolas llamamos $a$ a la distancia entre el centro y el vértice de la hipérbola, y $c$ seria la distancia del centro a un foco

- Igual que en todas las cónicas tenemos dos focos $F_1, F_2$ y el centro de la hipérbola esta en ${F_1 + F_2 \over 2}$ o extraído de su forma canónica $(h, k)$

- Podemos obtener la distancia $a$ gracias a la relación $|d(P, F_1)-d(P, F_2)| = 2a$

- Para calcular el valor de $c$ o de $b$ aplicamos Pitágoras $c^2 = a^2 + b^2 \rarr b^2=c^2-a^2$

- La distancia focal y excentricidad se calculan como en la elipse

- Las asintotas son rectas imaginarias a las que se acerca cada vez mas la hipérbola pero sin llegar a coincidir nunca. Dada una hipérbola ${x^2 \over a^2}-{y^2 \over b^2}=1$ las rectas $y={b \over a}x, y = -{b\over a}x$ son sus asintotas

- Es importante saber cual es el eje principal para pintar la hipérbola, esto lo sabemos porque el eje principal es la letra que acompaña la fracción positiva.

  Eje principal $x$: $({x - h \over a})^2 -({y - k \over b})^2 = 1$

  Eje principal $y$: $({y - k \over a})^2 -({x - h \over b})^2 = 1$

  Sabiendo esto sabemos que $a$ va con el eje principal, $b$ con el eje secundario y $c$ con el principal

#### Hiperbola equilatera

Una hipérbola es **equilátera** si se cumple cualquiera de las siguientes condiciones equivalentes: 

1. $a=b$
2. $c = a\sqrt2$
3. Su excentricidad es $\sqrt2$
4. Sus asíntotas son perpendiculares.

### Parábolas

Una parábola es el lugar geométrico de los puntos que tienen la misma distancia a un punto fijo (foco) que a una recta directriz. Es decir $d(P, F) = d(P, r)$

Ecuación canónica (hay 2): $y - k= {(x-h)^2 \over 4p}; x - h = {(y-k)^2 \over 4p}$

Se puede usar $2p$ o $4p$ indistintamente, normalmente se suele usar $4p$ siendo $p$ la distancia focal. Usando $2p$ requiere saber que $p$ es el parámetro en vez de la distancia focal.

#### Elementos de una parábola

![https://weeklymathblog.weebly.com/uploads/8/7/5/9/87593848/parabola-x_orig.png](https://weeklymathblog.weebly.com/uploads/8/7/5/9/87593848/parabola-x_orig.png)

---

- Vértice: $(h, k)$

- Dirección de la parábola: el termino elevado al cuadrado indica si la parabola es horizontal ($y$) o vertical ($x$). Sabiendo ya esto sabemos si abren hacia un lado u otro dependiendo de $p$.

  Ejemplo: $x^2=-4y$. Esta parabola es vertical y abre hacia abajo

- Hallar $p$, necesitamos en primer lugar saber si nos referimos a $p$ como:

  - Parametro: distancia del foco a la directriz
  - Distancia focal: distancia del foco al vertice

  Esto es importante porque nos puede confundir hacer calculos con $p$ como parametro que realmente es $2p$

- Para hallar el foco necesitamos saber la direccion, el vertice y el valor de $p$. Una vez tenemos todo esto y sabiendo que el foco queda por dentro de la parabola hacemos el calculo.

  Ejemplo: $x^2=-4y$. Su vertice es $(0, 0)$ abre hacia abajo, lo cual quiere decir que su vertice esta en $x = 0$ y su $y$ esta en $-1$. Ergo el foco es $(0, -1)$

- Directriz recta fija, esta a una distancia $p$ del foco pero fuera de la parabola.

  Ejemplo: $x^2=-4y$. Si su vertice es $(0, 0)$ y $p = -1$ la directriz es la recta $y= -(-1)$