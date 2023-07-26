### Transacciones con las bases de datos.

## Definicion
Una transacción es un bloque de sentencias SQL que se ejecuta como una sola, es decir, si por una razón una de las sentencias perteneciente al bloque falta, todas las demas se detendran automaticamente.

## Conceptos básicos
Las transacciones garantizan que se cumplan las propiedades ACID: atomicidad, consistencia, aislamiento y durabilidad, (atomicity, consistency, isolation, durability)

### Atomicidad
Asegura que toda la transacción se ejecute o no, de manera que el proceso nunca quede inconcluso.

### Consistencia
Asegura la coherencia antes y después de una transacción, por ejemplo, si se modifica un campo llamado amount en una tabla, cuyo valor inicial era el número 5, despues de la transacción dicho campo solamente debería tener valores numerícos y no cadenas de texto.

### Aislamiento
Garantiza que se puedan ejecutar varias transacciones al mismo tiempo, evitando que se generen inconsistencias en los datos.

### Durabilidad
Garantiza que una vez completada la transacción los datos sean almacenados de forma permanente.

## Motores de almacenamiento
