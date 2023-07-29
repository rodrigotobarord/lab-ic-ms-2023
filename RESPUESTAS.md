## ETAPA 1

¿Cuál es la diferencia entre los archivos con el verbo Create con los archivos con el verbo Add?

[R] Loas archivos con el verbo Create crean tablas. Los archivos con el verbo Add, insertan registros a las tablas creadas.

Revisa el contenido del archivo docker-compose.yml.

¿Cómo se llama el servicio que se declara en el archivo docker-compose.yml?

[R] El servicio se llama flyway

¿Cuál es el comando que se ejecuta en el servicio declarado?

[R] -locations=filesystem:/flyway/sql -connectRetries=60 migrate



## ETAPA 2

¿Qué pasa si cambias el nombre del servicio de postgres a db? ¿Qué otros cambios tendrías que hacer?

[R] Modificar la dependencia de flyway (depends_on) a db



## ETAPA 3

Revisa el archivo movies-api/Dockerfile.

¿Qué te llama la atención?

[R] Se agrega el servicio movies-api cuya imagen se construye

Revisa el archivo docker-compose.yml.

¿Cómo se relacionan el archivo docker-compose.yml y el archivo movies-api/Dockerfile?

[R] En movies-api/Dockerfile se encuentran las directivas para construir la aplicación movies-api, y docker-compose la llama para que al momento previo al despliegue se realice el build. 

¿Qué crees que hace el atributo context debajo de build (está en la linea 6 del archivo docker-compose.yml)?

[R] Ls ruta hacia donde va el docker-file
