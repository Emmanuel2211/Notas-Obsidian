---
type: zettel
date: "2026-09-05"
status: undone
aliases:
tags:
 - calculus
cssclasses: 
 - romana
---
# Funciones de Trigonometricas

> [!theorem] **Definición.** (Seno y Coseno)
> Sea $x \in \mathbb{R}$, definimos las funciones seno y coseno mediante las siguientes series, las cuales son absolutamente convergentes en todo $\mathbb{R}$.
> $$
> \begin{align}
> \sin(x) &= \sum_{n=0}^{\infty} \frac{(-1)^{n}}{(2n+1)!}x^{2n+1} = x - \frac{x^{3}}{3!} + \frac{x^{5}}{5!} -\dots \\[0.5em]
\cos(x) &=  \sum_{n=0}^{\infty} \frac{(-1)^{n}}{(2n)!}x^{2n} = 1 - \frac{x^{2}}{2!} + \frac{x^{4}}{4!} - \dots
> \end{align}
> $$



> [!theorem] **Teorema.** (Propiedades)
> 1. Derivadas: $\displaystyle \frac{d}{dx} \cos(x) = -\sin (x)$ y $\displaystyle \frac{d}{dx} \sin(x) = \cos(x)$.
> 2. $\sin ^{2}(x) + \cos ^{2}(x) = 1$.
> 


> [!theorem] **Definición.** ($\pi$)
> El número $\pi$ se define como el doble de la raíz positiva más pequeña de la función coseno. Es decir, $\displaystyle \frac{\pi}{2}$ es el único real en $(0,2)$ que satisface:
> $$
> \cos\left(\frac{\pi}{2}\right) = 0
> $$


> [!theorem] **Teorema.** (Limites de Trigonometricas)
> 1. 
> $$
> \lim_{ x \to 0 } \frac{\sin(x)}{x} = 1
> $$



> [!proof]- **Proof.**
> Por definición, para todo $x \neq 0$:
> $$
> \sin(x) = \sum_{n=0}^{\infty} \frac{(-1)^n}{(2n+1)!} x^{2n+1} = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + \dots
> $$
> Dividimos toda la serie entre $x$:
> $$
> \frac{\sin(x)}{x} = 1 - \frac{x^2}{3!} + \frac{x^4}{5!} - \frac{x^6}{7!} + \dots
> $$
> Queremos acotar el error de aproximación. Analizamos la diferencia:
> $$
> \left\vert{} \frac{\sin(x)}{x} - 1 \right\vert{} = \left\vert{} -\frac{x^2}{3!} + \frac{x^4}{5!} - \frac{x^6}{7!} + \dots \right\vert{}
> $$
> Para valores pequeños de $x$ (por ejemplo, $0 < \vert{}x\vert{} < 1$), esta es una serie alternante convergente donde los términos decrecen en valor absoluto. Por el Teorema de Estimación de Series Alternantes (o el residuo de Taylor), el valor absoluto de la suma completa está acotado por el valor absoluto del primer término:
> $$
> \left\vert{} \frac{\sin(x)}{x} - 1 \right\vert{} \le \left\vert{} -\frac{x^2}{3!} \right\vert{} = \frac{x^2}{6}
> $$
> Ahora, construimos la prueba formal con límites $\varepsilon-\delta$:Sea $\varepsilon > 0$. Elegimos $\delta = \sqrt{6\varepsilon}$ (y exigimos $\delta \le 1$).Si $0 < \vert{}x\vert{} < \delta$, entonces:
> $$
> \left\vert{} \frac{\sin(x)}{x} - 1 \right\vert{} \le \frac{x^2}{6} < \frac{\delta^2}{6} \le \frac{6\varepsilon}{6} = \varepsilon
> $$
> Como para todo $\varepsilon > 0$ existe un $\delta > 0$ que satisface la condición, por definición, el límite es $1$.
> $$
> \tag*{$\blacksquare$}
> $$
