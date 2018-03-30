A continuación, se muestran procedimientos y funciones para desarrollar servicios RESTful utilizando Oracle REST Data Services.

# Tabla de Cotenidos

+ ORDS.CREATE_ROLE
+ ORDS.CREATE_SERVICE
+ ORDS.DEFINE_HANDLER
+ ORDS.DEFINE_MODULE
+ ORDS.DEFINE_PARAMETER
+ ORDS.DEFINE_PRIVILEGE
+ ORDS.DEFINE_SERVICE
+ ORDS.DEFINE_TEMPLATE
+ ORDS-DELETE_MODULE
+ ORDS.DELETE_PRIVILEGE
+ ORDS.DELETE_ROLE
+ ORDS.DROP_REST_FOR_SCHEMA
+ ORDS.ENABLE_OBJECT
+ ORDS.ENABLE_SCHEMA
+ ORDS.PUBLISH_MODULE
+ ORDS.RENAME_MODULE
+ ORDS.RENAME_PRIVILEGE
+ ORDS.RENAME_ROLE
+ ORDS.SET_MODULE_ORIGINS_ALLOWED
+ ORDS.SET_URL_MAPPING


## ORDS.CREATE_ROLE
Crea un rol de ORDS con el nombre especificado.

```
ORDS.CREATE_ROLE ( 
    p_role_name IN sec_roles.name% type 
);
```

Ejemplo:
```
EXECUTE ORDS.CREATE_ROLE(
    p_role_name => 'Tickets User'
);
```

***

## ORDS.CREATE_SERVICE

Crea un servicio RESTFul.

```
BEGIN
    ORDS.CREATE_SERVICE(
        p_module_name => 'my.tickets',
        p_base_path => '/my/tickets/',
        p_pattern => '.',
        p_source => 'select t.id "$.id", t.id, t.title from tickets t' || 
            ' where t.owner = :current_user order by t.updated_on desc'
    );
END;
```

***

## ORDS.DEFINE_HANDLER

***

## ORDS.DEFINE_MODULE

```
BEGIN
    ORDS.DEFINE_MODULE(
        p_module_name => 'my.tickets',
        p_base_path => '/my/tickets/'
    );
END;
```

***

## ORDS.DEFINE_PARAMETER

Define un parámetro de controlador de módulo. Si el parámetro ya existe, entonces el parámetro será reemplazado por esta definición; de lo contrario, se crea un nuevo parámetro.
*** 

## ORDS-DELETE_MODULE 

***

¿Qué es una colección?

# Errores
```json
{
    "type": "http://www.w3.org/Protocols/rfc2616/rfc2616-sec10.html#sec10.5.1",
    "status": 500,
    "title": "ORA-06550: línea 2, columna 3:\n
            PLS-00201: el identificador 'DBMS_SODA_ADMIN' se debe declarar\n
            ORA-06550: línea 2, columna 3:\n
            PL/SQL: Statement ignored\n",
    "details": "begin\n DBMS_SODA_ADMIN.LIST_COLLECTIONS(\n P_START_NAME => ?,\n P_RESULTS => ?);\nend;", 
    "o:errorCode": "SQL-06550" 
}
```

https://www.databaseusers.com/article/6359253/PLS-00201%3A+identifier+'DBMS_SODA_ADMIN.LIST_COLLECTIONS'+must+be+declared.