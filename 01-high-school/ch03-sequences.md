# Sucesiones

Es una secuencia ordenada de números. Se representan como $\{1, 2,3,4, 5... \}$.

El termino general de una sucesión es el termino que ocupa el lugar n-ésimo, en el caso de la sucesión anterior es $a_n = n$ ya que para la posición $n$ el valor es $n$ también.

## Progresiones Aritméticas

Sucesión de números tales que cada uno de ellos (salvo el primero) es igual al anterior más un número fijo llamado diferencia que se representa por $d$.

Ejemplo: $\{2, 5, 8, 11, 14...\}$ tiene una diferencia de $+3$ ya que va de 3 en 3

Para hallar su termino general hay que aplicar $a_n = a_1 + (n-1)d$ por ejemplo en la sucesión anterior la regla general es $a_n = 3n -1$

NOTA: Cuidado con las progresiones de [números cuadrados y cúbicos](https://www.youtube.com/watch?v=F_rhZajOScc&feature=youtu.be)

La suma de los $n$ primeros términos de una progresión aritmética es $S_n = {n * (a_1 + a_n) \over 2}$

## Progresiones Geométricas

Cada termino se obtiene multiplicando el anterior por una razón $r$.

Ejemplo: $\{1, 2, 4, 8, 16...\}$ tiene una razón de $+2$ ya que cada termino es el anterior por este

Para hallar su termino general hay que aplicar $a_n = a_1 * r ^ {n-1}$ por ejemplo en la sucesión anterior la regla general es $a_n = 1 * 2 ^ {n-1}$

La suma de los $n$ primeros términos de una progresión geométrica es $S_n = {r*a_n-a_1 \over r-1}$

El producto de los $n$ primeros términos de una progresión geométrica es $P_n = \pm a_1 * r ^{n-1 \over 2}$

## Clasificación de sucesiones: convergente, divergente, oscilante

Para entender esto vendría bien refrescar el conocimiento de limites.

- Convergente: el limite de la sucesión tiende a un numero real
- Divergente: el limite de la sucesión tiende a $+\infin$ o $-\infin$
- Oscilante: sucesión sin limite

## Monotonía y acotación

Se dice que una sucesión es monótona cuando todos sus términos tienen un sentido estricto.

- Si $a_n < a_{n+1}$ entonces es monótona creciente
- Si $a_n > a_{n+1}$ entonces es monótona decreciente

Se dice que una sucesión esta acotada si se puede decir cual es su limite superior o inferior

## Fracción generatriz

Es la fracción irreducible que genera un numero decimal. Por ejemplo el numero $0,5 = 1/2$ por lo que $1/2$ es la fracción generatriz de $0,5$.

Podemos usar las sucesiones para obtener la fracción generatriz de un numero periódico sabiendo que la suma de un número ilimitado de términos de una progresión geométrica de primer termino no nulo viene dada por: $S = {a_1 \over 1-r}$ siempre y cuando $|r| < 1$

Cogiendo el numero $2,\overgroup{37} = 2 + {37 \over 100} + {37 \over 100*100} + {37 \over 100 * 100 *100}+...$

Los términos periódicos forman una progresión geométrica de razón $r = {1\over100}$

Podemos calcular la suma infinita de los términos de esta progresión y sumarle la parte entera y decimal no periódica (si tiene).

$2 + {{37\over100}\over{1- {1\over100}}} = 2 + ({37\over100} : {99\over100}) = 2 + {37\over99} = {198\over99} + {37\over99} = {235\over99}$

Y nos queda que ${235\over99}$ es la fracción generatriz de $2,\overgroup{37}$

## Capitalización compuesta

Si depositamos en una entidad financiera una cantidad de dinero $C_0$ durante un tiempo $t$ y un rédito $r$, obtendremos un beneficio $I = C_0·r·t$ llamado interés. (es importante que el rédito y el tiempo estén en la misma unidad, años, meses, días...)

Off-topic: La diferencia entre interés simple y compuesto es que en el compuesto se acumulan tus ganancias en el banco y generan un interés en base al nuevo dinero y en el simple el dinero se da año a año sin la posibilidad de acumularse para generar mas.

Al final del primer año tendremos $C_1 = C_0 + I = C_0 + (C_0 * r * 1) = C_0 * (1+r)$

El capital final obtenido después de *n* años dado un capital inicial *C0* y un rédito *r* dado en tanto por
uno, es: $C_t =C_0 * (1+r)^t$

## Limites

Es el estudio de una función, expresión algebraica o sucesión en una situación extrema.

El infinito no es un numero, es un concepto que indica números muy grandes positivos o negativos.

Veamos el $=$ como un "tiende a":

- $n * \infin = \infin$
- $n / \infin = 0$
- $n + \infin = \infin$
- $n - \infin = \infin$
- $\infin / \infin = Indeterminacion$
- $\infin - \infin = Indeterminacion$
- $1 ^ \infin = Indeterminacion$
- $\infin^2 = \infin$
- SOLO EN LIMITES: $n/0 = \infin$

[Video explicando límites aplicados a sucesiones.](https://youtu.be/39Q1ZwI9cFY)

## Logaritmos

Un logaritmo se define como $log_b a = x \rarr b^x = a$. Tenemos que encontrar el exponente al que elevada la base $b$ de como resultado el argumento $a$. (si no tiene base la base es $10$)

Para hallar el logaritmo de un numero hay que ponerlo con forma exponencial ($b^x = a$) y después operamos. IMPORTANTE: [Repasar las propiedades de los radicales.](https://www.youtube.com/watch?v=Cfl8HcObbGA)

Ejemplo: $log_5(0,2) \rarr 5^x = 0,2 \rarr 5^x = {2\over10} \rarr 5^x = {1\over5} \rarr 5^x = 5^{-1}$

[Logaritmos neperianos](https://youtu.be/CiuYq3gNK-o)

### Propiedades de los logaritmos

- Logaritmo de 1 es 0 (cualquier base)
- Un logaritmo con misma base y mismo argumento es 1
- $log (a * b) = log (a) + log(b)$
- $log (a / b) = log (a) - log(b)$
- $log (a ^ b) = b * log (a)$