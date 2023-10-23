Si bien un array puede contener cualquier lista en muchos casos es necesario especificar restricciones sobre los  ítems del mismo. Para ello se utiliza la palabra clave items. Por ejemplo si quisíeramos que todos los elementos de un array sean de tipo numérico deberíamos escribir algo así.

" edades " :{ " type " : " array " ," items " :{ " type " : " integer " }}

En ese tipo de situaciones puede ocurrir que no  
todos los elementos del array sean del mismo tipo y además puede pasar que no  
querramos ítems extras mas allá de los que definimos.

" direccion " : {  
	" type " : " array " ,  
	" items " : \[  
		{ " type " : " string " } ,  
		{ " type " : " number " } ,  
		{ " type " : " string " } ,  
		{ " type " : " string " }  
		 \] ,  
	" additionalItems " : false  
}

El tamaño máximo y mínimo de un array puede  
establecerse especificando a minItems y maxItems. Un arreglo que tenga entre 8  
y 10 elementos se especifica as ́ı:


" integrantes " : {  
	" type " : " array " ,  
	" minItems " :8 ,  
	" maxItems " : 10  
}

Pero además podríamos indicar que cada elemento debe ser único utilizando la palabra clave uniqueItems  
" integrantes " : {  
	" type " : " array " ,  
	" minItems " :8 ,  
	" maxItems " : 10 ,  
	" uniqueItems " : true  
}