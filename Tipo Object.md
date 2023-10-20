Este tipo se utiliza para declarar documentos y documentos embebidos.Para el ejemplo de la secci´on 1.3 tenemos el documento principal que representa a un cliente y un documento anidado que representa a la direcci´on

{ 
	" type ": " object ", 
	" properties " :{ 
		" nombre " :{" type ":" string " } ,
		 " apellido " :{" type ":" string " },
		  " fecha_nacimiento " :{" type ":" string "," format ":"date - time "} ,
		   " direccion " :{
			    " type ":" object ", 
			   " properties " :{
				    " calle " :{" type ":" string " } , 
				    " ciudad " :{" type ":" string " } ,
				     " pais " :{" type ":" string " } 
				}
			 }
		 }
	 }
El tipo object tiene un conjunto de propiedades (properties) que son definiciones de pares clave-valor. Cada propiedad a su vez tiene su propio tipo que puede ser otro object. Las propiedades de un object no son necesariamente exhaustivas, un documento con una propiedad extra tambi´en es v´alido a no ser que se especifique lo contrario. Para evitar propiedades adicionales se usa additionalProperties con el valor false. additionalProperties es un objeto que adem´as puede establecer condiciones sobre las propiedades adicionales. Por ejemplo en direcci´on podr´ıamos permitir agregar propiedades s´olo de tipo string
