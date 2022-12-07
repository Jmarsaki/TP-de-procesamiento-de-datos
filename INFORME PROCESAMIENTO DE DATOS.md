# TP-de-procesamiento-de-datos
Trabajo práctico de procesamiento de datos
Trabajo práctico de procesamiento de datos. La consigna es:
 Nos contrata una agencia de autos para que descarguemos mensualmente la lista de precios de los vehículos. Página oficial de ACARA.

Nuestro sistema tiene una tabla de 3 columnas, mtm_id clave, anio_modelo clave y fecha que es la última actualización. (nombre de las columnas lo puede redefinir)

Tomar en cuenta si quieren una tabla histórica para no hacer el control de fecha.

tareas

Procesar la información recibida y generar un procedimiento escrito y simulado de cómo deberían ser las secuencias para dicha tarea.

Deben tomar en cuenta:

Repositorio del archivo
Responsable de la ejecucion
Proceso
Resultado impacto en la tabla.
Control de duplicados
Control de no pisar valores en cero o blanco
La tabla debe estar en una base de datos relacional, en teoría esta tabla puede llegar a tener 1,5 millones de registros:
una. MySQL/Maria DB
b. PosgreSQL
C. Servidor MSSQL/Sybase
d. Oráculo
Queda a su criterio que herramientas van a utilizar para el procesamiento
 Para realizar este trabajo se trabajo con Power bi. Los pasos a seguir fueron:  
1- Se sube el archivo en .csv y con la función "transformar datos" se realizan los siguientes pasos;
a- Se transforman los valores "null" de todas las columnas en cero.
b- Se elimina la fila superior con los nombres de las variables de cada columna.
c- Se toma la primera columna "mtm_id clave" y se usa la función "dinamización de las otras columnas" para reducir la tabla a tres columnas.
d- Se borran los valores cero y quedan vacías las casillas correspondientes.
e- Se usa la función "borrar filas con casillas vacías", cortando la tabla.
f- Se pueden ordenar los valores según ascendente o descendente desde alguna de las columnas (ejemplo: anio_modelo). Asi queda lista la tabla solicitada.
2- Se guarda dicha tabla en una base de datos determinados. Por cuestiones de equipo obsoleto, si bien específicamente GitHub no es base de datos, puede cumplir la función de guardar la tabla y por ello se elije el mismo.

¡¡GRACIAS!!
