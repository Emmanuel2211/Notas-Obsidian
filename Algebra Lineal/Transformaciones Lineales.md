---
type: zettel
status: 
links: 
tags: []
date: "2026-05-21"
aliases: [ "transformacion lineal" ]
cssclasses: romana
materia: 
---
# Transformaciones Lineales

> [!theorem] **Definición.** (Transformacion Lineal)
> Sean $V$ y $W$ esp. vect. sobrem $\mathbb{F}$. Una función $T: V \to W$ se llama **transformación lineal** de $V$ en $W$ si $\forall x,y \in V$ y $c \in  \mathbb{F}$ tenemos que
> 1. $T (x + y) = T(x) + T(y)$ 
> 2. $T(cx) = cT(x)$


> [!observation]- **Observaciones.**
> Sea $T: V \to W$ demostrar:
> - Si $T$ es lineal, ent. $T(0) = 0$
> - $T$ es lineal sii $T(ax + y) = aT(x) + T(y) \quad \forall x,y \in V \ \forall a \in \mathbb{F}$
> - $T$ es lineal si y sólo si para $x_{1},\dots,x_{n} \in  V$ y $a_{1},\dots,a_{n}\in \mathbb{F}$ tenemos que
> $$
> T(\sum_{i=1}^{n} a_{i}x_{i}) = \sum_{i=1}^{n} a_{i}T(x_{i})
> $$ 


> [!example]- Ejemplo.
> Sean $V$ y $W$ esp. vect. sobre $\mathbb{F}$,
> - Definimos la **transformación identidad** $| : V\to V$ mediante $|_{V}(x) = x \quad \forall x \in  V$.
> - Definimos la transformación cero $T_{0}: V \to W$ por $T_{0}= 0 \quad \forall x \in  V$.

el rango y el kernel

> [!theorem] **Definición.** (Kernel)
> Sean $V, W$ esp. vect. y sea $T: V \to  W$ lineal. Definimos al **espacio nulo** o **kernel** $N(T)$ de $T$ como el conjunto de todos los vectores $x \in  V$ tales que $T(x) = 0$.
> $$
> N(T) = \{ x \in V \mid T(x) = 0 \}
> $$


> [!theorem] **Definición.** (Rango)
> Sean $V,W$ esp. vect. y sea $T: V\to W$ lineal. Definimos al **rango** o **imagen** $R(T)$ como el subconjunto de $W$ que consta de todas las imágenes (bajo $T$) de los elementos de $V$, es decir
> $$
> R(T) = \{ T(x) \mid x \in V\} 
> $$


> [!theorem] **Teorema.**
> Sea $V$ un esp. vect. y $W_{1}$ un subespacio de $V$. Sea $T$ una proyección sobre $W_{1}$, y sea $W_{2}$ tal como en la definición de proyección. Entonces
> $$
> W_{1} = R(T) \quad \text{ y } \quad W_{2} = N(T)
> $$


algo de que genera al rango (teorema)

> [!theorem] **Teorema.** (Teorema de la Dimensión)
> Sean $V$ y $W$ esp. vect. sobre $\mathbb{F}$ y sea $T:V\to W$ lineal. Si $V$ tiene dim. finita, Ent. 
> $$
> \operatorname{dim} (V) = \operatorname{dim} (N(T)) + \operatorname{dim} (R(T))
> $$

> [!proof]+ **Proof.**
> Sup. que $\operatorname{dim} (V) = n$. Por el Teo. de dim. de subespacios, $\operatorname{dim} (N(T)) \leq n$. Llamemos $k = \operatorname{dim} (N(T))$, $k\leq n$.
> Sea $\beta_{0} = \{ v_{1},\dots,v_{k} \}$ una base de $N(T)$. Por un Cor. del Teo. de Reemplazo, podemos extender $\beta_{0}$ a una base de $V$, digamos $\beta = \{ v_{1},\dots,v_{k},v_{k+1},\dots,v_{n} \}$
> **PD.** $\langle T[\{ v_{k+1},\dots,v_{n} \}] \rangle = R(T)$
> Sabemos que, por el Teo. anterior,
> $$
> R(T) = \langle T[\beta ] \rangle = \langle \{ T(v_{i}) : 1\leq i \leq n \} \rangle
> $$
> Como $\forall i \in  \{ 1,\dots,k \} \ (v_{i} \in  N(T))$, tenemos que $R(T) = \langle \{ T(v_{i}) : 1 \leq i \leq n \} \rangle = \langle \{ \bar{0} \cup \{ T(v_{i} : k+1 \leq i \leq  n) \} \} \rangle$
> $$
> = \langle \{ T(v_{i}) : k+1 \leq  i \leq n \} \rangle
> $$
> **PD.** $\{ T(v_{i}) : k + 1 \leq  i \leq  n \}$ es l.i.
> Sean $a_{k+1} , \dots , a_{n} \in  \mathbb{F}$ tq $\displaystyle \sum_{i=1}^{n} a_{i} T(v_{i}) = \bar{0}_{W}$.
> **PD.** $\forall  i \in  \{ k+1, \dots, n \} ( a _{i} = 0_{\mathbb{F}})$
> $$
> \bar{0}_{W} = \sum_{i=k+1}^{n} a_{i}T(V_{i}) = T(\sum_{i=k+1}^{n} a_{i}v_{i})
> $$
> Así, $\displaystyle \sum_{i=k+1}^{n} a_{i}v_{i} \in N(T)$
> Luago existen $b_{1},\dots,b_{k} \in  \mathbb{F}$ tq
> $$
> \sum_{i=1}^{k} b_{i}v_{i} = \sum_{i=k+1}^{n}  a_{i}v_{i}
> $$
> Ent.
> $$
> \bar{0}_{V} = \sum_{i=1}^{k} -b_{i}v_{i} + \sum_{i=k+1}^{n} a_{i}v_{i}
> $$
> Como $\beta = \{ v_{1},\dots,v_{k}, v_{k+1}, \dots,v_{n} \}$ es base de $V$, 
> $\forall i \in  \{ k+1,\dots,n \}\ (a_{i} = 0)$.
> $$
> \therefore \text{ el cjto. es l.i. }
> $$
> **PD.** $\forall  i , j \in  \{ k+1,\dots,n \} \ (i\neq j \implies T(v_{i}) \neq T(v_{j}))$
> Sean $i,j \in \{ k+1,\dots,n \}$. Sup. $i\neq j$, ent. $v_{i} \neq  v_{j}$.
> Sup. $T(v_{i}) = T(v_{j})$, ent. 
> $$
> \bar{0}_{W} = T(v_{i}) - T(v_{j}) = T(v_{i}-v_{j})
> $$
> Luego $v_{i}-v_{j} \in  N(T)$. 
> Entonces existen $a_{1},\dots,a_{k} \in  \mathbb{F}$ tq
> $$
> \begin{align}
> v_{i}-v_{j} &= \sum_{\ell=1}^{k} a_{\ell}v_{\ell} \\[0.5em]
> \bar{0}_{V} &= \sum_{\ell=1}^{k} a_{\ell}v_{\ell} + (-1)v_{i} + 1v_{j}
\end{align}
> $$
> Esto es una comb. lineal no trivial del $0$ con elementos de la base $\beta$!
> Contradicción
> $$
> \therefore T(v_{i}) \neq  T(v_{j})
> $$


---


> [!theorem] **Teorema.** (Representación Matricial)
> Una transformación **lineal** $T : \mathbb{R}^n \to \mathbb{R}^m$ admite una representación mediante la matriz $A_{T} \in M_{m\times n}$, en el sentido de que $\forall \mathbf{x} \in \mathbb{R}^n : T (\mathbf{x}) = A_{T}\cdot \mathbf{x}$
> Donde $A_{T}$ se llama **matriz estándar** de $T$, y se define como
> $$
> A_{T} = \begin{pmatrix}
> T(\mathbf{e_{1}}) &  \dots & T(\mathbf{e_{n}})
> \end{pmatrix}_{m\times n}
> $$
> Claro, $\mathbf{e}_{k}$ son los canónicos

> [!theorem] **Teorema.** (Recíproco del teorema anterior)
> Toda matriz $A \in M_{m\times n}$ genera una transformación lineal
> $$
> T_{A} : \mathbb{R}^n \to \mathbb{R}^m
> $$
> tal que $A \cdot \mathbf{x} = T_{A}(\mathbf{x})$


**Prop.** La composición de transformaciones lineales, es de nuevo una transformación lineal.

**Prop.** Si $T_{1},T_{2}: \mathbb{R}^n \to \mathbb{R}^n$ son transformaciones lineales y $A_{1},A_{2} \in M_{n\times n}(\mathbb{R})$ son sus respectivas matrices estándar, entonces
$$
\begin{align}
A_{T_{2} \circ T_{1}} = A_{T_{2}} \cdot A_{T_{1}} \\[0.5em]
A_{T_{1} \circ T_{2}} = A_{T_{1}} \cdot A_{T_{2}}
\end{align}
$$



---
#### Algunas transformaciones lineales útiles
Sobre transformaciones lineales **elementales.**

**Rotaciones:** 
$$
T_{\varphi} \begin{pmatrix}
x \\
y 
\end{pmatrix} = \begin{pmatrix}
\cos \varphi & -\sin \varphi \\
\sin \varphi & \cos \varphi
\end{pmatrix} \begin{pmatrix}
x \\
y
\end{pmatrix}
$$

**Reflexiones:**
$$
T_{m} \begin{pmatrix}
x \\
y
\end{pmatrix} = \frac{1}{1+m ^{2}} \begin{pmatrix}
1-m^{2} & 2m \\
2m & m^{2}-1
\end{pmatrix} \begin{pmatrix}
x  \\
y
\end{pmatrix}
$$
Contra el eje $X$:
$$
T_{X} \begin{pmatrix}
x \\
y
\end{pmatrix} = \begin{pmatrix}
1 & 0 \\
0 & -1
\end{pmatrix} \begin{pmatrix}
x \\
y
\end{pmatrix}
$$
Contra el eje $Y$:
$$
T_{Y} \begin{pmatrix}
x \\
y
\end{pmatrix} = \begin{pmatrix}
-1 & 0 \\
0 & 1
\end{pmatrix} \begin{pmatrix}
x \\
y
\end{pmatrix}
$$
Contra $y = x$:
$$
T_{y = x} \begin{pmatrix}
x \\
y
\end{pmatrix} = \begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix} \begin{pmatrix}
x \\
y
\end{pmatrix}
$$

**Compresión-Dilataciones:** Por un factor $r$ a lo largo de un eje coordenado.
$$
T \begin{pmatrix}
x \\
y
\end{pmatrix} = \begin{pmatrix}
rx \\
y
\end{pmatrix} = \begin{pmatrix}
r & 0 \\
0 & 1
\end{pmatrix} \begin{pmatrix}
x \\
y
\end{pmatrix}
$$
$$
T \begin{pmatrix}
x \\
y
\end{pmatrix} = \begin{pmatrix}
x \\
ry
\end{pmatrix} = \begin{pmatrix}
 1 & 0 \\
 0 & r
\end{pmatrix} \begin{pmatrix}
x \\
y
\end{pmatrix}
$$

**Deslizamientos Relativos:** Por un factor $r$ a lo largo de un eje coordenado.
$$
T \begin{pmatrix}
x \\
y
\end{pmatrix} = \begin{pmatrix}
 x + ry \\
 y
\end{pmatrix} = \begin{pmatrix}
1 & r \\
0 & 1
\end{pmatrix} \begin{pmatrix}
x \\
y
\end{pmatrix}
$$
$$
T \begin{pmatrix}
x \\
y
\end{pmatrix} = \begin{pmatrix}
x \\
rx + y
\end{pmatrix} = \begin{pmatrix}
1 & 0 \\
r & 1
\end{pmatrix} \begin{pmatrix}
x \\
y
\end{pmatrix}
$$

Continuamos con el criterio de diagonalización^[[[Diagonalizacion]]]
