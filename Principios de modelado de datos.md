1. Know your data: La primera clave de n diseño correcto de una base de datos es entender los datos, esto se captura mediante modelo conceptual de datos. (i.e hacer el DER). 
2. know your queries. los tipos de consultas que se le pueden hacer a una DB, afectan el diseño de la misma. Se definen 3 tipos de acceso distintos: 
	1. partición por consulta: la opción más eficiente es cuando una consulta busca una sola fila, un conjunto de filas o todas las filas de una sola partición. 
	2. partición+ por consulta : buscar datos de varias particiones de una tabla. 
	3. tabla o tabla+ por consulta:  buscar datos de varias particiones de varias tablas
3. Data nesting: agrupa múltiples entidades en base a algún criterio. 
4. data duplication: Duplicating data in Cas-  
sandra across multiple tables, partitions, and rows is a common  
practice that is required to efficiently support different queries  
over the same data. It is far better to duplicate data to enable  
the “partition per query” access path than to join data from  
multiple tables and partitions. For example, to support queries  
Q1 and Q2 in Fig. 3(b) via the efficient “partition per query”  
access path, we should create two separate tables that organize  
the same set of artifacts using different table primary keys. In  
the Cassandra world, the trade-off between space efficiency  
and time efficiency is almost always in favor of the latter.