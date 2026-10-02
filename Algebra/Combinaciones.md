---
type: zettel
date: "2026-07-03"
aliases:
tags: 
 - algebra
cssclasses: 
 - romana
---
# Combinaciones

> Ahora, interpretemos en lugar de listas, sacos!
> ¿Cuántos "sacos" de $m$ elementos podemos hacer? Sea un conjunto $\left| A \right| = n$.
> $$
> A = \{ a,b,c,d \}
> $$
> y queremos subconjuntos de $2$ elementos. Claramente $\lvert A \rvert = 4$.
> Se tendrá que
> $$
> O^{4}_{2} = \frac{4!}{2!} = \text{ Listas posibles }
> $$
> $$
> \text{ Num. Listas } = (2!)(\text{ Num sacos })
> $$
> $$
> \implies  \text{ Num. sacos } = \frac{\text{ Num listas }}{2!} = \frac{4!}{2! (2!)}
> $$

En general,


---

> [!theorem] **Definición.** (Combinación)
> Sea $A$ un cjnt. sean $n,m \in  \mathbb{N}$ tales que $0\leq m\leq n$. Una $m$**-combinación de** $A$ es cualquier subconjunto de $A$ que tenga exactametne cardinalidad $n$. Denotamos al número de **combinaciones de** $A$ **tomados de** $m$ **en** $m$ como
> $$
> C_{m}^{n} = \begin{pmatrix}
> n \\
> m
> \end{pmatrix} = \frac{n!}{m!(n-m)!}
> $$

En calculadoras: $nCm$, $nPm$, $nOm$

> [!example]- Ejemplo.
> Poker: $52$ cartas, $4$ palos, $13$ números. Una mano $= 5$ cartas al azar.
> $\Omega =$ Todas las posibles manos.
> $$
> \left| \Omega  \right| = C_{5}^{52} = \frac{52!}{5! (47!)} = 2,598,960
> $$
> Manos destacadas:
> 1. Flor real: $A,10,J,Q,K$ del mismo palo. Su cardinalidad es 4, pues solo hay 4 palos.
> $$
> P[\text{ Flor real  }] = \frac{4}{2,598,960}
> $$

Investigar cuales son las manos destacadas.
