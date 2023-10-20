Para tipos n´umericos puede usarse integer para valores enteros o number para otros.

{
" edad " : {" type ": " integer "} , 
" sueldo " :{" type ": " number "}
}

El tipo integer no es un tipo propio de JavaScript y por ende de JSON, por lo cual puede provocar confusi´on. Desde el punto de vista de la especificaci´on puede quedar m´as o menos claro qu´e entendemos por integer aunque un documento puede tener 1 y 1.0 y ambos ser considerados v´alidos. El tipo number indica cualquier n´umero incluso en notaci´on exponencial.

Como en el caso de los strings, los n´umeros puede ser restringidos. Para restringir n´umeros hay dos formas establecer: m´ultiplos o rangos.


1. multiplos { " edad " :{" type ":" number "," multipleOf ":1.0} , }
2. Rangos { " edad " : {" type ": " integer "} , " sueldo " :{" type ": " number ", " minimum ":7800 , " maximum ": 78000 , " exclusiveMinimum ": true } }