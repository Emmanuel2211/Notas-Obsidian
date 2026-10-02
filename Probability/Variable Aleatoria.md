---
type: zettel
date: "2026-09-01"
status: undone
aliases:
tags:
 - probability
cssclasses:
 - romana
---
# Variable Aleatoria


> [!theorem] **Definición.** (Variable Aleatoria)
> Una variable aleatoria, denotada $X$, es una función $X: \Omega \to \mathbb{R}$ tal que para cualquier $x \in  \mathbb{R}$,
> $$
> \{ \omega \in \Omega \mid X(\omega ) \leq x \} \in  \mathcal{F}
> $$
>
> Sea $A \in \mathcal{B}(\mathbb{R})$ cjto. boreliano, denotamos $(X \in A)$ como la imagen inversa de $A$
> $$
> (X \in  A) = X^{-1}(A) = \{ \omega  \in  \Omega  \mid  X(\omega ) \in A \}
> $$

La variable aleatoria, no es ni variable, ni aleatoria, es una función determinista, que relaciona resultados $\omega$ con número $\mathbb{R}$. Sin embargo, *su nombre se justifica al considerar que los posibles resultados del experimento son los valores de la funcíon* $X$. Vemos ejemplos para tener esto claro:

Como $(X \in  A) \in  \mathcal{F}$, podemos sacar la medida de proba $P[A]$ para $A \in \mathcal{B}(\mathbb{R})$. Es decir, podemos **inducir** la medida de proba a intervalos de la forma $(-\infty, x]$, y en general, a ciertos números $\mathbb{R}$ pertenecientes a $\mathcal{B}(\mathbb{R})$.


> [!example]- Ejemplo.
> Sea $A = (x,y)$, considerando $(X \in  A)$ podemos también escribirlo de la forma $( x < X < y )$, es decir
> $$
> (X \in (x,y)) = \{  \omega  \in  \Omega  \mid  x < X(w) < y \}
> $$
> De misma forma $(X \in (-\infty,x])$ es $(X \leq  x)$, es decir
> $$
> (X \in (-\infty,x]) = \{ \omega \in  \Omega  \mid X(w) \leq x  \}
> $$
> Y este último es una condición muy especial (*condición de medibilidad*), notese que está en nuestra definición de Variable Aleatoria.


> [!Info]- Medida de Probabilidad Inducida
> Sea cualquier intervalo de la forma $(-\infty,x]$, por medio de su imagen inversa $X^{-1}((-\infty,x])$ se puede aplicar la medida de probablidad $P$, pues su $X^{-1}$ está en $\mathcal{F}$ (dada nuestra definición). Así, mediante una variable aleatoria $X$ puede tomarse la proba $P$ de $A \in  \mathcal{B}(\mathbb{R})$. En ocaciones se le denota $P_{X}$, llamada **medida de proba inducida por la variable aleatoria** $X$. Así pues, tenemos un nuevo esp. de proba. de interés $(\Omega , \mathcal{B}(\mathbb{R}), P)$.


> [!theorem] **Definición.** (Función Indicadora)
> La variable aleatoria en la cual, sea $A$ evento, toma el valor $1$ si $A$ ocurre o es $0$ si $A$ no ocurre, es llamada **función indicadora**, denotada:
> $$
> \mathbb{1}_{A}(w) = \begin{cases}
  1 & w \in A \\[0.5em]
  0 & w \not\in A
\end{cases}
> $$


---

> Es una función que asigna un real a cada resultado de un experimento.

> [!example]- Ejemplo.
> Queremos saber la cantidad de aguilas que salieron en 4 lanzamientos de una moneda. Esto podríamos definirlo como una función $X: \Omega \to \mathbb{R}$ tal que para cada $\omega  \in  \Omega$ se define $X(\omega ) = \# \text{ de ágilas en } \omega$.
> Al ser función, tenemos que su imágen directa es, sea $B \subseteq \mathbb{R}$.
> $$
> X^{-1}[B] = \{ \omega  \in  \Omega \mid X(\omega ) \in B  \}
> $$
> En este experimento tenemos que $B = \{ x \}$, con $x \in  \mathbb{N}$ (el núm. de ágilas), es decir
> $$
> X^{-1}[\{ x \}] = \{ \omega \in \Omega \mid X(\omega ) = x \}
> $$
> Observese que $X^{-1}[\{ 2 \}]$ está en $\mathcal{F}$ (*sigma-álgebra*), por lo que le podemos asignar una proba.
 


> [!theorem] **Definición.** (Variable Aleatoria)
> Sea $(\Omega , \mathcal{F}, P)$ un espacio de probabilidad. Una **variable aleatoria** $X$ es una función medible $X: \Omega  \to  \mathbb{R}$ tal que para cada $B \in  \mathcal{B}(\mathbb{R})$ se cumple que $X^{-1}[B] \in  \mathcal{F}$.
> 
> Es decir, $X$ es una variable aleatoria si la imagen inversa bajo $X$ de cualquier evento del $\sigma$-álgebra de Borel, es un evento de $\mathcal{F}$.




> [!theorem] **Definición** (Soporte de una V.A.)
>
>


> [!theorem] **Definición.** (Función de Densidad)
> $P[X =a] = f_{x} (a)$
> se llama función de densidad de $X$.


Veremos algunas funciones de densidad especiales:

Jacob Bernoulli, en otros casos son otros Bernoullis, su familia hizo muchas cosas.
1. Bernoulli: Es una v.a para eventos con dos posibles resultados

$$
\Omega = \{ \text{Exito} , \text{Fracaso} \} = \{ A, A^{c} \}
$$
Definimos a la v.a. Bernoulli como $X= 0$ sii ocurre fracaso. $X = 1$ si ocurre Exito.
Entonces, $P[X = 0] = P[\text{ Fracaso }] = P[A^{c}]$ y $P[X = 1] = P[\text{ Exito }] = P[A]$
Entonces:
$$
f_{x}(a) = \begin{cases}
  P & a=1 \\
(1-P) & a= 0 \\
0 & \text{ c.o.c }
\end{cases}
$$
$= p^{a}(1-p)^{1-a}; a \in \{ 0,1 \}$
$= p^{a}(1-p)^{1-a}\cdot \mathbb{I}^{(a)}_{\{ 0,1 \}}$
implicitamente o explicitamente (con la funcion indicadora)
$$
\mathbb{I}_{\{ 0,1 \}}(a) = \begin{cases}
  1  & a \in  \{ 0,1 \} \\[0.5em]
  0 & a  \not\in \{ 0,1 \}
\end{cases}
$$
> [!theorem] **Definición.** (Función Indicadora)
> $$
> \mathbb{I}_{A}(a) = \begin{cases}
  1 & a \in A \\[0.5em]
  0 & a \not\in A
\end{cases}
> $$

En resumen, si $X$ es una v.a. Bernoulli:
$$
f_{x}(a) = p^{a}(1-p)^{1-a}\mathbb{I}_{\{ 0,1 \}}(a)
$$
y el $\operatorname{Sop}_{x} = \{ 0,1 \}$
Notación: $X \sim \operatorname{Ber} (p)$ Se lee, $X$ es una v.a. Bernoulli con proba de exito $p$.

2. Uniforme

Notación: $X \sim \operatorname{UnifDis} (n)$
$X$ es una v.a uniforme y el número de resultados es $n$?

Es una v.a. para experimentos con $n$ resultados los cuales tienen la misma proba.
$\Omega = \{ R_{1},\dots,R_{n} \}$
$\operatorname{Sop} _{x} = \{ 1,2,\dots,n \}$
$\implies f_{x}(a) = p[x=a] = \frac{1}{n} \quad a \in  \{ 1,n \}$
$$
= \frac{1}{n} \mathbb{I}_{\{ 1,2,\dots,n \}} (a) = \begin{cases}
  \frac{1}{n} & a \in \{ 1,\dots,n \} \\[0.5em]
0 & \text{ c.o.c. } 
\end{cases}
$$


---

###### Referencias

- https://blog.nekomath.com/proba1-variables-aleatorias/
