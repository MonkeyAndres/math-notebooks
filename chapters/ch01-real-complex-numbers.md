# Números reales y complejos

## Tipos de números

Diferentes conjuntos de números:

- Naturales (1, 2, 3, 4, ...)
- Enteros (..., -3, -2, -1, 0, 1, 2, 3, ...)
- Racionales: se pueden expresar como fracción y su expresión decimal es exacta o periódica
- Irracionales: no se pueden expresar como fracción, expresión decimal no periódica e infinita
- Reales: Racionales + Irracionales

Los números reales cumplen que son densos, esto significa que entre cada dos números reales hay infinitos números también reales. ([explicación](https://www.youtube.com/watch?v=fLzlbgxisUg))

---

El valor absoluto se utiliza para definir cantidades y distancias en el mundo real ya que como sabemos no existen cantidades ni distancias negativas.

---

La distancia en la recta real nos sirve para calcular distancias entre números reales, por ejemplo: "Si estamos en el sótano 9o y subimos al piso 5o, ¿Cuántos pisos hemos subido?". 

$Dist(-9, 5) = | -9 - 5 | = 14$

## Intervalos y entornos

Un intervalo de números reales es un conjunto de números correspondientes a una parte de la recta numérica.

Tipos de intervalos:

- Abierto: los extremos no forman parte del intervalo

  $I = (a, b)$

- Cerrado: los extremos forman parte del intervalo

  $I = [a, b]$

- Semiabierto: uno de los dos extremos no forma parte de la recta

  $I = (a, b]$

  $I = [a, b)$

Un entorno es una forma especial de expresar intervalos abiertos. (`a` centro, `r` radio)

Entorno a intervalo: $E(a, r) = (a-r, a+r)$

Intervalo a entorno: $(b, c) = E((b+c)/2, (c-b)/2)$

## Cálculo de errores

Error Absoluto: $EA = | valor real - valor aproximado |$

El Error Relativo se usa para comparar errores de distintas magnitudes o numeros, se suele multiplicar por 100 para hablar de % de error realtivo. Formula: $ER = EA / |valor real|$

## Notación científica

La notación científica se usa para expresar números muy grandes o números muy pequeños. Consta de: $N = a,bcd... *10^n$

- Parte entera de una sola cifra
- Parte decimal de x cifras
- Una potencia de base 10 y exponente n. Dependiendo de si el exponente es positivo o negativo se deduce si el numero es muy grande o muy pequeño

Para operar con números dados en notación científica se procede de forma natural, teniendo en cuenta que cada número está formado por dos factores: la expresión decimal y la potencia de base 10.

- Para **multiplicar** números en notación científica, se multiplican las partes decimales y se suman
  los exponentes de la potencia de base 10.
- Para **dividir** números en notación científica, se dividen las partes decimales y se restan los
  exponentes de la potencia de base 10.
- Si hace falta se multiplica o se divide el número resultante por una potencia de 10 para dejar
  con una sola cifra en la parte entera.

Ejemplo: $(3’7 * 10^6) * (4’2 * 10^8) = (3’7 * 4’2) * 10^{6+8} = 15’54 * 10^{14} = 1’554 * 10^{15}$

- Para sumar o restar números en notación científica, hay que poner los números con la misma potencia de base 10, multiplicando o dividiendo por potencias de base 10.
- Se saca factor común la potencia de base 10 y después se suman o restan los números decimales quedando un número decimal multiplicado por la potencia de 10.

Ejemplo: 

$3’7*10^9+4’2*10^{12} =3’7*10^9+4200*10^9 =(4203’7)*10^9=4’2037*10^{12}$

## Números complejos

Los números complejos o imaginarios se crearon para resolver ecuaciones imposibles por ejemplo la famosa ecuación $x^2 + 1 = 0$. Para esto se inventa un numero $i$. Esto es el teorema fundamental del álgebra.

Los números complejos se expresan como $z = x + iy$ a esto se le llama forma binomica, donde:

- $x$ es la parte real. $Re(z) = x$
- $y$ es la parte imaginaria. $Im(z) = y$

Los números complejos con parte imaginaria a 0 son números reales y los con parte real a 0 son números imaginarios.

Dos números complejos son iguales si tienen su parte real e imaginaria igual.

### Operaciones en forma binómica

- Suma, resta y multiplicación exactamente iguales que en números reales siguiendo reglas de álgebra
- División, se multiplica el numerador y denominador por el conjugado (cambiar el + por - en forma binomica) del denominador para conseguir un denominador con $i^2$ que es igual a $-1$

Calcular el binomio de newton: [explicación](https://www.youtube.com/watch?v=UUtQCUukD7Q).

---

### Representación en plano

Para representar números complejos en un plano solo tenemos que tener en cuenta la forma binomica y representar en el eje normal el valor de $x$ y de $y$.

Al representar no se representan en un plano normal con eje de abscisas (y) y eje de ordenadas (x). Se representan con un eje real (parte real, x) y eje imaginario (parte imaginaria, y)

---

### Modulo y argumento

El modulo o el valor absoluto de un numero complejo es $|Z| = \sqrt {x^2 + y^2}$ indica la distancia desde el origen al punto que representa el numero complejo

Argumento de un numero complejo es $arg(Z) = arctg(y/x)$ esto nos da un resultado en radianes (entre $-π/4$ y $π/4$ ) o en grados (entre -45º y 45º) por la función $arctg$. A esto hay que realizarle un ajuste dependiendo del cuadrante en el que se encuentre nuestro numero, simplemente dibuja gráficamente el numero y mira cuantos radiales o grados hay que sumarle para moverlo a su cuadrante.

Para obtener el $Arg$ o argumento principal hay que saber un argumento común y consiste en reducir el mismo argumento (substrayendo $2π$ que es el equivalente a quitar una vuelta entera) hasta que este en el rango comprendido entre $[-π, π)$ o $(-π, π]$.

Si tenemos por ejemplo un argumento $arg(Z) = \frac {5 π} {4}$ y queremos saber su argumento principal habría que hacer $Arg(\frac {5π} {4}) = \frac {5π} {4} - 2π = \frac {5π} {4} - \frac {8π} {4} = -\frac {3π} {4}$

Aquí tienes una mejor [explicación](https://m.youtube.com/watch?v=Xrles8Mwk0M) de los argumentos de un numero complejo. 

---

### Forma polar y forma trigonométrica

Para representar un numero complejo en forma polar solo necesitamos haber calculado su modulo y su argumento y lo expresaríamos como: $Z = |Z| * e ^ {i*α}$. (siendo $α$ un argumento en grados)

Para representar un numero complejo en forma trigonométrica tenemos que calcular el modulo y el argumento y representarlo como la siguiente formula $Z = |Z| (cos(α) + sen(α)i)$

Para volver de vuelta a la forma binómica simplemente hay que simplificar la forma trigonometría

### Operaciones entre números complejos en forma trigonométrica

- Multiplicar: multiplicar sus módulos y sumar los argumentos

  $z1 * z2 = (pr)(cos(α+ Θ) + i*sen(α+ Θ))$

  Si se pasan de 360º la suma de los ángulos podemos reducirlos para que pertenezcan a (0,360]º

- Dividir: dividir sus módulos y restar argumentos

  $z1 * z2 = (p/r)(cos(α - Θ) + i*sen(α - Θ))$

- Potencia: se eleva el modulo a la potencia y se multiplica el argumento por el exponente

  $Z^n = r^n (cos(α * n) + i*sen(α * n))$

- [Raíz enésima de un complejo](https://www.youtube.com/watch?v=4RZsTGklX0U): tiene como resultado tantos números complejos como el exponente de la raíz. La primera raíz se calcula con: $\sqrt[n]Z = \sqrt[n] {r*e^{(\alpha * i) /n}}$

  Una vez calculada la primera raíz se puede calcular la separación: $360 / n$

  Y ahora habría que hacer $\sqrt[n] {r*e^{(\alpha * i /n)+separacion}}$