---
type: zettel
date: "2026-08-19"
status: undone
aliases:
 - 
tags:
 - calculus
cssclasses: 
 - romana
---
# Trigonométricas Hiperbólicas

Después de construir $\exp \left(x\right)$, definimos sus partes: par e impar. 
> Recordamos que toda función real puede escribirse como la suma de una función par y una impar, las hiperbólicas son justo esto para $e^{x}$ .

> [!theorem] **Definición.** (Funciones Hiperbólicas)
> Sea $x \in  \mathbb{R}$, definimos:
> - $\displaystyle \sinh(x) = \frac{e^{x}- e^{-x}}{2}$
> - $\displaystyle \cosh(x) = \frac{e^{x}+ e^{-x}}{2}$
> - $\displaystyle \tanh(x ) = \frac{\sinh(x)}{\cosh(x)} = \frac{e^{x}-e^{-x}}{e^{x}+e^{-x}}$

A partir de las propiedades de $\exp \left(x\right)$ (*leyes de exponentes*), demostramos el casi análogo del Teorema de Pitágoras.

> [!theorem] **Teorema.** (Identidad Fundamental Hiperbólica)
> $$
> \cosh^{2}(x) - \sinh^{2}(x) = 1
> $$


##### Graficas

> [!observation]+ **Observación.**
> Dado $e^{2}x > 0$, $\cosh(x) > 0$ para todo $x$, lo que significa que por el teorema anterior
> $(\cosh(x), \sinh(x))\in \{ x^{2} - y^{2} = 1, x > 0 \}$, esto representa a la "rama positiva de la hipérbola $x^{2} - y^{2} = 1$".

para graficar, necesitamos sacar la derivada, evaluar decreimentos y crecimientos.
concavidades, convexidades... ver si es simetrica, ejes de simetria y punto de simetrica, si es par o impar,
veremos que es una funcion catenaria

![[Pasted image 20260906133906.png|center|383]]


##### Derivadas

##### Funciones Inversas

> [!theorem] **Teorema.** (Funciones Inversas Trigonometricas)
> Sea $x \in \mathbb{R}$,
> - $\displaystyle \sinh^{-1}(x) = \log \left(x+ \sqrt{x^{2}+1}\right)$
> - $\displaystyle \cosh^{-1}(x) = \log \left(x + \sqrt{x^{2} -1}\right)$
> - $\displaystyle  \tanh^{-1}(x) = \frac{1}{2}\log \left(\frac{1+y}{1-y}\right)$
> - $\displaystyle  \operatorname{ctgh}^{-1}(x) = \frac{1}{2}\log \left(\frac{1+y}{y-1}\right)$
> - $\displaystyle \operatorname{sech}^{-1}(x) = \log \left(\frac{1+ \sqrt{1 - y^{2}}}{y}\right)$
> - $\displaystyle \operatorname{csch}^{-1}(x) = \log \left(\frac{1 + \sqrt{1 + y^{2}}}{y}\right)$


Demostrar que son inversas, encontrar dominio, graficarlas

---

Demostradas las propiedades de los exponentes y de la funcón exponencia, podemos abrir la discución



> [!theorem] **Teorema.** (Propiedades)
> - Identidad Fundamental
> $$
> \cosh ^{2} \theta - \sinh ^{2} \theta = 1
> $$
> - Derivadas:
> $$
> \begin{align}
> \sinh' (x) &= \cosh(x) \\[0.5em]
> \cosh' (x) &= \sinh(x) \\[0.5em]
> \tanh'(x) &= \frac{1}{\cosh ^{2} (x)} \\[.5em]
> \coth'(x) &= \frac{1}{\sinh ^{2} (x)}\\[0.5em]
> \operatorname{sech}' (x) &= -\tanh (x) \operatorname{sech} (x) \\[0.5em]
> \operatorname{csch}' (x) &= -\coth(x)\operatorname{csch}(x)
> \end{align}
> $$
> - Derivadas de Funciones Inversas:
> $$
> \begin{align}
> \sinh ^{-1}(y) = \log(y+\sqrt{ y^{2} + 1 }) \\[0.5em]
> d
> \end{align}
> $$
> - jfdk
> $$
> \sinh( x) + \sinh (y) = 2 \sinh \left( \frac{x+y}{2} \right) \cdot \cosh \left(\frac{x-y}{2} \right)
> $$
> - fjkd
> $$
> \begin{align}
> 2\sinh ^{2}\left( \frac{x}{2} \right) &= \cosh(x) - 1 \\
> 2\cosh ^{2} \left( \frac{x}{2} \right) &= ? TAREA
> \end{align}
> $$



> [!proof]- **Proof.** 
> e

