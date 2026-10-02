---
type: zettel
tags: 
- sets
date: "2026-06-09"
aliases: 
- ZF
cssclasses: 
- romana
---

# Axiomas Zermelo-Fraenkel (ZFC)


Es importante tener la noción de **clase** como *objeto* de ZF^[[[Classes (conjuntos)|Clases]]]

> [!theorem] **Axiom de Existencia.** *Existe un conjunto que carece de elementos,* $\varnothing$.

> [!theorem] **Axiom de Extensionalidad.**^[[[Axioma de Extensionalidad]]] *Si $X$ y $Y$ tienen los mismo elementos, entonces $X = Y$*.



> [!theorem] **Axiom of Pairing (emparejamiento).**^[[[Axioma de Emparejamiento]]] *For any $a$ and $b$ there exists a set $\{ a,b \}$ that contains exactly $a$ and $b$*.

> [!theorem] **Axiom Esquema de Separación.**^[[[Axioma de Separacion]]]  *Si $P$ es una propiedad (con parámetro $p$), entonces para cualquier $X$ y $p$ existe un conjunto $Y = \{ u \in X : P(u,p) \}$ que contiene todo $u \in X$ con la propiedad $P$*.

^28a139


> [!theorem] **Axiom of Union.**^[[[Axioma de Union]]] *For any $X$ there exists a set $Y = \bigcup X$, the union of all elements of $X$.*

> [!theorem] **Axiom of Power.**^[[[conjunto potencia|Axioma de Potencia]]] For any $X$ there exists a set $Y = P(X)$, the set of all subsets of $X$.

> [!theorem] **Axiom of Infinity.** *There exists an infinite set.*

> [!theorem] **Axiom Schema of Replacement** (Esquema axiomático de reemplazo). *If a class $F$ is a function, then for any $X$ there exists a set $Y = F(X) = \{ F(x) : x \in X \}$.*

> [!theorem] **Axiom of Regularity.** *Every nonempty set has an $\in$-minimal element.*

> [!theorem] **Axiom of Choice.** *Every family of nonempty sets ahs a choice function. (the C in ZFC)*

Hay teoría de conjuntos con axiomática Zermelo-Fraenkel (ZF); y (ZFC) que es ZF con axioma de elección (AC).
