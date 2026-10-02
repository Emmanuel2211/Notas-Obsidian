---
type: zettel
date: 2026-09-23
status: undone
aliases:
tags:
  - calculus
cssclasses:
  - romana
---
# Polinomio de Taylor

> [!theorem] **Definición.** (Polinomio de Taylor)
> Sea $I \subseteq \mathbb{R}$ un intervalo abierto y $a \in  I$. Sea $f: I\to \mathbb{R}$ función $n$-veces diferenciable en $a$. El **polinomio de Taylor de grado $n$ centrado en** $a$ denotado $P_{n,a}(x)$ es
> $$
> P_{n,a}(x) = \sum_{k=0}^{n} \frac{f^{(k)}(a)}{k!} (x-a)^k
> $$
> Desglosado, esto es:
> $$
> P_{n,a}(x) = f(a) + \frac{f'(a)}{1!}(x-a) + \frac{f''(a)}{2!}(x-a)^2 +\frac{f'''(a)}{3!}(x-a)^3 + \dots + \frac{f^{(n)}(a)}{n!}(x-a)^n
> $$
>
> Si $a = 0$, es conocido como polinomio de Maclaurin.



