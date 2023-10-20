Un JSON Schema es un documento JSON que describe la estructura de otro documento.

{ " type ": " object ",
	" properties " : { " nombre " : {" type ":" string " } ,
	 " apellido " : {" type ":" string " } ,
	  " fecha_nacimiento " :{" type ":" string "," format ":"date - time "} ,
	  " direccion " :{ 
			  " type ":" object ", 
			  " properties " :{ " calle " :{" type ":" string " } ,
			   " ciudad " :{" type ":" string " } ,
			    " pais " :{" type ":" string " }
			}
		}
	 }
 }

1.  [[Palabra clave type]]
2. [[metadata title, description y default]]
3. [[Tipos]]
4. 
