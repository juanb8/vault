![[Pasted image 20231020192830.png]]

1. MR1 (Entidades y relaciones):  entidades y tipo de relaciones se mapean a tablas.  Entidades y relaciones se mapean a las filas de una tabla.  Atributos que describen a las entidades y  a las relaciones, se mapean a columnas.![[Pasted image 20231020192941.png]]
2. MR2 (atributos de búsqueda de igualdad): Equality search at-  
tributes, which are used in a query predicate, map to the prefix  
columns of a table primary key. Such columns must include all  
partition key columns and, optionally, one or more clustering  
key columns. Violation of this rule may result in inability to  
support query requirements.![[Pasted image 20231020193259.png]]
3. MR3 I(nequality search attributes): An inequality search  
attribute, which is used in a query predicate, maps to a table  
clustering key column. In the primary key definition, a column  
that participates in inequality search must follow columns that  
participate in equality search. Violation of this rule may result  
in inability to support query requirements![[Pasted image 20231020193514.png]]
4. MR4  (Ordering Attributes). Ordering attributes, which are  
specified in a query, map to clustering key columns with  
ascending or descending clustering order as prescribed by the  
query. Violation of this rule may result in inability to support  
query requirements.![[Pasted image 20231020193559.png]]
5. MR5 (Key Attributes). Key attribute types map to primary  
key columns. A table that stores entities or relationships as  
rows must include key attributes that uniquely identify these  
entities or relationships as part of the table primary key to  
uniquely identify table rows. Violation of this rule may lead  
to data loss.![[Pasted image 20231020193645.png]]
