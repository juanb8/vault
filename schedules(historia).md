Es una secuencia de [[transacciones]]. Lo importante que hay que entender es que estas transacciones se hacen en memoria buffer, es decir se hace un `read(A)` , se opera con los datos y luego se hace un `write(A)` para guardarlos. E problema surge si se quiere hacer esto concurrentemente. ![[Pasted image 20231023132022.png]]
Una historia puede ser [[serial schedules (historia serial)]] y una historia puede ser [[serializable schedule (historia serializable)]]. 

