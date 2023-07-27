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
Un motor de almacenamiento se define como el encargado de almacenar, gestionar y recuperar los datos guardados en las tablas.  
La sentencia para ver el listado de motores de almacenamiento es: <b>SHOW ENGINES;</b>

InnoDB es el motor de almacenamiento por defecto a partir de la version 8 de MySQL, sin embargo es posible cambiarlo.

### Ver motores de almacenamiento.
````sql
SHOW ENGINES;
````

### Definir un motor de almacenamiento diferente a InnoDB
````sql
CREATE TABLE nombre_tabla (
    "campos" INT NOT NULL
) ENGINE = motor_almacenamiento;
````

### Sentencia para cambiar el motor de almacenamiento establecido en una tabla.
````sql
ALTER TABLE nombre_tabla
ENGINE = motor_almacenamiento;
````

## Motores de almacenamiento

Motor de almacenamiento
- InnoDB

Caracteristicas
- Soporta transacciones
- Bloquea datos a nivel de regitro y no bloquea las lecturas durante el proceso SELECT
- Se recupera de caídas
- Se limitan las columnas a un máximo de 1000.
- Almacena un máximo de 64 Tb por tabla.
- No permite indices FULLTEXT
- Es complicado cambiar la ubicacion de la base de datos.

## Estrctura de una transacción

1. Comienza la transacción con el uso de la sentencia BEGIN o START TRANSACTION.
2. Escribe el bloque de sentencias que se quiere ejecutar, ya sea INSERT, DELETE, UPDATE.
3. Ejecuta la sentencia COMMIT para completar la transacción (considera que todos los cambios serán permanentes)
4. Ejecuta la sentencia ROLLBACK para revertir los cambios hechos en caso de un fallo.

### Sentencia para ejecutar una transacción.
````sql 
START TRANSACTION 
"sentencias a ejecutar"
COMMIT;
````
