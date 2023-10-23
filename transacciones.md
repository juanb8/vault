$T_i \subseteq \{w_i(X); r_i(X)\}\cup \{c_i,a_i\}$
1. $T_1$ es la transacción $i$ y $<i$ es el orden parcial
2. $w_i(X)$ es el write de la transacción $i$  del ítem $X$
3. $r_i(X)$ es el read de la transacción $i$  del ítem $X$
4. $c_i$ commit
5. $a_i$ abort
6. $a_i \in T \iff c_i \notin T_i$
