El tipo string se refiere a cadenas de caracteres undicode. Una propiedad de tipo string puede tener como valor cualquier cadena de caracteres. Para poder limitar los valores posibles existen otras palabras claves asociadas a string. 

Para establecer restricciones respecto a la longitud de un string se utilizan las palabras claves: minLength y maxLength.

" codigo " :{" type ": " string ", " minLength ": 5," maxLength ": 15 }

Tambi´en es posible establecer que un string debe cumplir con una expresi´on regular con la sint´axis de las expresiones regulares de JavaScript. Se utiliza la palabra clave pattern como se ve en el siguiente c´odigo:

{ " email " : {" type ": " string ", " pattern ":"^\w+@\[a-zA -Z_ \]+?\ .\[a-zA -Z\]{2,3}$" } }

Es importante notar el uso de ”∧ ” al comienzo y de ”$” al final porque sino la expresi´on regular se eval´ua si aparece en cualquier parte de la cadena. La expresi´on regular del ejemplo permite establecer el formato de un correo electr´onico, pero para ello JSON Schema provee un m´etodo m´as simple para establecer la validaci´on sem´antica de strings y es utilizar la palabra clave format. Hay un grupo de formatos preestablecidos:

“date-time” Fecha seg´un el RFC 3339 

“email” correo electr´onico 

“hostname” Nombre de host de internet seg´un el RFC 1034 

“ipv4” Direcci´on IP versi´on 4 o IPv4 

“ipv6” Direcci´on IP versi´on 6 o IPv 

“uri” Identificador universal de recurso (URI) seg´un el RFC3986. 

Utilizando format el ejemplo del correo electr´onico puede escribirse:

{ " email " : {" type ": " string ", " format ":" email " } } 