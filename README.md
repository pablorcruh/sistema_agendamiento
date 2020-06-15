# SISTEMA DE AGENDAMIENTO

## Descripción

El presente proyecto funciona por el mommento con dos ambientes 
para la base de datos 

* Un ambiente para H2 llamado **dev** 
* Un ambiente para conexión con mysql llamado **test**

Usamos un contenedor para la base de datos mysql, el siguiente comando
no permite configurar el contenedor
 ```
docker run --name mysql -p 3306:3306 -v /path/to/folder/data:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=example -d mysql:5.7

```
El projecto usa Liquibase para la migración de scripts de base de
datos
