Dos operaciones son  **conflictivas** si operan sobre el mismo ítem y al menos una es un `write`.

Dos historias ($H_i, H_j$) son **conflicto equivalente**  sí 
1. Están definidas sobre el mismo conjunto de transacciones
2. El orden de las operaciones conflictivas de transacciones no abortadas es el mismo.
Otra definición, dos historias son **conflicto equivalente** si podemos convertir una en otra por una secuencia de `swaps` de acciones adyacentes. 

Una historia $H$ es conflicto **serializable(SR)** si es conflicto equivalente a alguna historia serial $H \equiv H_s$

Ejemplo, tenemos la historia, ![[Pasted image 20231023140024.png]]
Se puede mostrar que es serializable si mostramos `swaps` de acciones adyacentes que los hace equivalente a una historia serial. ![[Pasted image 20231023140119.png]]
