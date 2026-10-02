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
# Variable Aleatoria Discreta




> [!theorem] **Definición.** (V.A. Discreta y Soporte)
> Sea $X$ una v.a. sobre $(\Omega ,\mathcal{F},P)$, diremos que es una **variable aleatoria discreta** si el conjunto de valores que puede tomar $X$, o sea $\operatorname{Im} \{X\}$, es **finito** o **infinito numerable**.
>
> Un conjunto $\mathcal{S}_{X} \in  \mathcal{B}(\mathbb{R})$ es llamado un soporte de la v.a. $X$ si
> $$
> P(X\in \mathcal{S}_{X}) = 1
> $$ 
> Así $X$ es una v.a. discreta si tiene un soporte finito o numerable. También denotamos a $\mathcal{S}_{X}$ como $\operatorname{supp}(X)$.




> [!theorem] **Definición.** (Función de Densidad o Probabilidad)
> Sea $X$ una v.a. discreta con valores $x_{0},x_{1}, \dots$ La función de proba de $X$, denotada $f_{X}: \mathbb{R} \to \mathbb{R}$ se define como
> $$
> f_{X}(x) = \begin{cases}
  P(X = x) & x = x_{0},x_{1}\dots \\[0.5em]
  0 & \text{ en otro caso }
\end{cases}
> $$
> Otra forma de escribirlo, $\forall x \in \operatorname{Im} \{X\}$
> $$
> f_{X}(x)  = P(X=x)
> $$ 

> [!observation]+ **Observación.**
> De nuestra definción, ahora podemos saber la proba de una evento $A$ por medio de la suma de la función de proba de todos sus elementos $x \in A$, esto es
> $$
> P(X \in A) = \sum_{x \in A} f_{X}(x) 
> $$
> Así, la función de densidad $f_{X}$ muestra la forma en la que la probabilidad $P$ se distribuye sobre el conjutno de puntos $x_{0},x_{1}\dots$, es decir, sobre $\operatorname{Im} \{X\}$.


Directamente, tenemos las siguiente propiedades de $f_{X}$

> [!theorem] **Teorema.** (Propiedades)
> Sea $X$ una v.a. discreta sobre $(\Omega ,\mathcal{F},P)$, se cumple que
>
> 1. $\displaystyle f_{X}(x) \geq  0 \quad \forall  x \in  \mathbb{R}$
> 2. $\displaystyle \sum_{x} f_{X}(x) =1$

