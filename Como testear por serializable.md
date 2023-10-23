Cuando un par de acciones en conflicto aparece es la historia $S$, las transacciones que performan esas acciones tienen que aparecer en el mismo orden en cualquier historia serial equivalente. Si esto no es contradictorio, podemos encontrar una historia serial equivalente.  Si son contradictoria entonces no tiene equivalente.  

Sea $S$ una historia que contiene las transaciones $T_1, T_2$ . Decimos que $T_1$ tiene **predecencia por sobre** $T_2$ ($T_1 <_S T_2$)  sí existen acciones $A_1$ y $A_2$ tales que: 
1. $A_1$  está adelante de  $A_2$ en $S$
2. Ambos accionan sobre el mismo elemento de la base de datos
3. algúno es un `write`
Por lo tanto una historia serial equivalente tiene $T_1$ antes de $T_2$. 
 
Una historia $H$ es serializable sí su [[Grafo de precedencia]] es acíclico. 

$H \in SR \iff SG(H)$ es acíclico. 

Sí $SG(H)$ es acíclico entonces los órdenes seriales es equivalente al **orden topológico del grafo**. 

 