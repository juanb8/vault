 MR1: Las entidades y las relaciones. 
	id_artifact
	title_artifact
	\[authors\]
	{keywords}
	name_venue
	year
MR2: Son clave lo que participa en  las consultas de igualdad
	id_artifact
	title_artifact
	\[authors\]                  K
	{keywords}
	name_venue
	year
Lo que tenemos es un arreglo de autores. Si ponemos la clave así es implica que ese arreglo de autores todo es la clave y es lo que no queremos.   El paper dice que pongamos un autor por separado y lo hagamos por el. 
MR2: 
	author                       K
	id_artifact
	title_artifact
	\[authors\]                  
	{keywords}
	name_venue
	year
MR3: 
	author                       K
	year                           C$\uparrow$
	id_artifact
	title_artifact
	\[authors\]                  
	{keywords}
	name_venue
MR4: 
	author                       K
	year                           C$\downarrow$
	id_artifact
	title_artifact
	\[authors\]                  
	{keywords}
	name_venue 
MR5: 
	author                       K
	year                           C$\downarrow$
	id_artifact                 C$\uparrow$
	title_artifact
	\[authors\]                  
	{keywords}
	name_venue 

