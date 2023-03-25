Tarea:

1) Pasar CSV a una nueva DB
2) Usar una REST ful API para que el servidor tenga nueva data. Un  servicio.
2.1) Cada transaccon debe encajar con las reglas del diccionario de datos.
2.2) Se debe poder ingestar transacciones batch (hasta 1000 registros) en un solo pedidos
2.3) En un mismo servicio debo poder recibir datos o ingestar por cada tabla.
2.4) tener en cuenta siempre las reglas de cada tabla.
3) Crear una funcionalidad para backup de cada tabla y salvarla en el filesystem en avro format.
4) Crear una funcionalidad para restablecer desde ese backup.
5) publicar codigo en github, para ir viendo las actualizaciones que se hicieron en el repositorio asi vemos el proceso del desarrollo.
6) Aquellas transacciones que no cumplen las reglas no deben insertarse, pero si deben estar logeadas.
7) Todos los campos son requeridos.

COSAS A ENTENDER:
0) puedo usar Python java go scala.
1) Yo decido el origen de los CSV
2) Yo decido el destino de la Base de datos.
3) el CSV es un archivo de comas separado.
4) Las funcionalidades pueden ser interpretados como "rest api, stored procedure, Funcionalidad de la DB, Cron Job, o otro camino que resuelva el requerimiento".

No es excluyente, pero se tendrá en cuenta:
1) Crear un archivo Readme.md
2) Seguridad en el servicio de API 
3) Usargit workflow para crear versiones
4) Crear un dockerfile para deployar el package
5) Usar herramientas cloud en vez de herramientas locales.

Herramientas vistas para hacer el proyecto:
1)Google colab
2)Trino (open source y docker)
3) dbt


Yendo por trino:
1)Ya existe en docker una imagen, descargar:

