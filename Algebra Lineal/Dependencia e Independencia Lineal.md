---
type: zettel
date: "2026-09-03"
status: undone
aliases:
tags:
 - algebra
cssclasses: 
 - romana
---
# Dependencia e Independecia Lineal

> Retomando nuestra motivación, una pregunta super importante es: ¿Cual de los subcjts. $S \subseteq V$ tal que $\langle S \rangle = W$, es el más chico (**con respecto a la contención propia**)? 
>
> Es decir habŕa algún $S' \subsetneq S$ tal que $\langle S' \rangle = \langle S \rangle$?
>
> Para resolverlo, nos planteamos ¿Será que algún vector de $S$ se puede escribir como comb. lineal de los demás?
> 

Antes de pasar a nuestra definiciones, tenemos que tener en mente como se puede describir a $\bar{0}$ como comb. lineal. Puede pasar que, sea $\{ u_{1},u_{2},u_{3} \} \subseteq  V$.
$$
\bar{0} = 2u_{1} + 0u_{2} + 5u_{3} \quad \text{ o que } \quad \bar{0} = 0u_{1} + 0u_{2} + 0u_{3}
$$
A la segunda, le llamamos *comb. lineal trivial* del $\bar{0}$.

> [!observation]+ **Observación.**
> Sean $\{ u_{1},\dots, u_{k} \}$, en ocasiones no sabemos que todos sean distinitos, al menos que se especifique que $i \neq j \implies  u_{i} \neq  u_{j}$. **Aguas!** Podemos pensar que encontramos una comb. lineal no trivial del $\bar{0}$ y NO sea así!
> $$
> \text{ Si } \ u_{1} = u_{2}, \implies  \bar{0} = 1u_{1} - 1u_{2} + 0u_{3}  +\dots + 0u_{k}
> $$

> [!theorem] **Definición.** (Comb. Lineal no Trivial del $\bar{0}$)
> Sea $V$ un esp. vect. sobre $\mathbb{F}$. Sea $S \subseteq V$ y $S \neq \varnothing$. Decimos que existe una **combinación lineal no trivial del $\bar{0}$ de vectores de** $S$ si y śolo si $\exists k \in  \mathbb{N}^{+} \ \exists u_{1},\dots,u_{k} \in  S \ \exists a_{1},\dots,a_{k} \in  \mathbb{F}$  tales que $\forall i,j \in \{ 1,\dots,k \} (i\neq j \implies  u_{i}\neq u_{j})$ y
> $$
> \exists i \in \{ 1,\dots,k \} (a_{i} \neq  0) \ \text{ y } \ \sum_{i=1}^{k} a_{i}u_{i} = \bar{0}
> $$


> [!theorem] **Lemita**
> Sea $V$ esp. vect. sobre $\mathbb{F}$ y $S \subseteq V$. Si $\bar{0} \in  S$, ent. existe una comb. lineal no trivial del $\bar{0}$ de vectores de $S$.



> [!theorem] **Definición.** (Dependencia Lineal)
> Sea $V$ esp. vect. sobre $\mathbb{F}$. Sea $S \subseteq V$. $S$ es **linealmente dependiente** (l.d) si y sólo si, hay un número finito no vacío de vectores en $S$, $x_{1},x_{2}, \dots, x_{k}$ distintos por pares y hay $a_{1}, \dots, a_{k} \in  \mathbb{F}$, no todos cero, tal que $\displaystyle \hat{0} = \sum_{i=1}^{k} a_{i}x_{i}$
> 
> Es decir,
> Sea $S \subseteq V$. $S$ es **l.d.** si y sólo si, $\exists k \in  \mathbb{N} ^{+} \ \exists x_{1}, \dots , x_{k} \in  S \ \exists a_{1}, \dots, a_{k} \in  \mathbb{F}$ de forma  que $\forall i,j \in  \{ 1,\dots,k \} (i\neq  j \implies x_{i} \neq  x_{j})$ y $\exists  i \in  \{ 1,\dots,k \} \ a_{i} \neq  0$ y
> $$
> \hat{0} = \sum_{i=1}^{k} a_{i}x_{i}
> $$
> 
> Y en español,
> $S\subseteq V$ es l.d. si y sólo si existe una combinación lineal no trivial de $\bar{0}$ usando vectores distintos por pares de $S$.


> [!theorem] **Definición.** (Independencia Lineal)
> Sea $S \subseteq V$. Decimos que $S$ es **linealmente independiente** (l.i.) si y sólo si **no** es l.d... AAAAHHH!


> Ya en serio, ¿Qué es realmente l.i.? Está gacho sólo decir que no es l.d.
 

> [!theorem] **Definición.** (Independencia Lineal)
> Sea $S \subseteq V$. $S$ es **l.i.** sii $\forall k \in  \mathbb{N}^{+} \ \forall x_{1},\dots,x_{k} \in  S \ \forall a_{1},\dots,a_{k} \in  \mathbb{F}$
> $$
> \forall i,j \in \{ 1,\dots k \} \left( (i\neq j \implies  x_{i} \neq x_{j}) \land \sum_{i=1}^{k} a_{i}x_{i} = \bar{0} \right)
> $$
> $$
>  \implies \forall i\in \{ 1,\dots k \} (a_{i} = 0)
> $$
>
> En español,
> $S\subseteq V$ es **l.i.** si y sólo si no hay una combinación lineal no trivial del $\hat{0}$ utilizando vectores de $S$ distintos.


> [!example]+ **Ejemplos.** 
> - $\varnothing$ es l.i. por vacuidad.
> - Si $S \subseteq V$ tal que $\bar{0} \in S$, ent. es l.d.
> - Si $S = \{ x \}$ con $x \neq \bar{0}$, $S$ es l.i.

> [!theorem] **Lema.** *Bonito*
> Sean $S_{1}, S_{2} \subseteq  V$, con $S_{1}\subseteq S_{2}$.
> 1. Si $S_{1}$ es l.d, ent. $S_{2}$ es l.d. (los l.d.s suben)
> 2. Si $S_{2}$ es l.i, ent. $S_{1}$ es l.i. (los l.i.s bajan)

> [!proof]+ **Proof.** Tarea


Formalizando un resultado muy importante,

> [!theorem] **Teorema.** (Teorema de la Linealidad Finita)
> Sea $V$ un esp. vect. y sea $S \subseteq V$ **finito** no vacío. Sea $n \in  \mathbb{N}^{+}$ tal que $\left| S \right| = n$ y sea $S = \{ v_{1},\dots,v_{n} \}$
> Ent. $S$ es **l.i.** si y sólo si
> $$
> \forall a_{1}, \dots, a_{n} \in  \mathbb{F} \ \left(\sum_{i=1}^{n} a_{i} v_{i} = \hat{0} \implies  \forall i \in  \{ 1,\dots,n \} (a_{i} = 0)\right)
> $$

> [!observation]- **Observación.**
> Gracias a que $P \iff Q \equiv  \neg P \iff  \neg Q$, el teorema anterior también aplica para l.d.'s finitos!

> [!proof]+ **Proof.**
> 

El siguiente resultado deberia de ser un Teorema por su importancia:

> [!theorem] **Teorema.** (Lema de Dependencia)
> Sea $S$ un subcjto. l.i. de un esp. vect. $V$. Sea $v \in  V$ tal que $v \not\in S$. Ent. $v \in  \langle S \rangle$ si y sólo si $S \cup \{ v \}$ es l.d.
>

> [!proof]+ **Proof.**
>
