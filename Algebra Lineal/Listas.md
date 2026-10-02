# TDA Listas

> En la vida diaria usamos listas para ordenar una sucesión de objetos. Ej. lista de compras, alumnos de un grupo, invitados o tareas...
>
> Ahora, nos preguntamos ¿Cómo podemos modelar este comportamiento?


> [!theorem] **Definición.** (Lista)
> Sea $\mathcal{L_{A}}$ el conjunto de las listas sobre un conjunto $A$, sea $x$ cualquier elemento (**cabeza**) y sea $xs$ el resto de elementos ya almacenados (**cola**) se cumple:
> 1. $[ \ ] \in  \mathcal{L_{A}}$ 
> 2. $xs  \in  \mathcal{L_{A}} \implies x : xs \in \mathcal{L_{A}}$
>
> Donde $x:xs$ es la operación "Inserta $x$ al inicio de la lista $xs$".

> [!example]- Ejemplo.
> Sea $A = [ \ ]$ sean $y,p,q$ elementos. Como $A \in  \mathcal{L_{A}}$:
> Insertamos $y : [ \ ] = [y]$
> Insertamos $p : [ y ] = [p,y]$
> Insertamos $q : [p,y] = [q,p,y]$
> Tenemos $[q,p,y]$ pero en realidad esto es $q : ( p : (y  : [ \ ]))$

![[Nota 9 Listas.pdf]]

