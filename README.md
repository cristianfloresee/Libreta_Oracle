## Instalación del Oracle Instant Client

http://www.oracle.com/technetwork/database/enterprise-edition/downloads/112010-win64soft-094461.html

Para acceder a una base de datos Oracle, necesita disponer de información tales como drivers, archivos y configuraciones Oracle. Para hacer esto, tienes dos opciones:

+ Instala a un cliente de base de datos Oracle.
+ Instala un Oracle Instant Client.

Se recomienda Instant Client, ya que podemos ejecutar nuestras aplicaciones (en este caso Toad) sin tener que instalar el cliente estándar de Oracle, que consume mucho más espacio.

La 'instalación' del Oracle Instant Client en realidad consiste en copiar unos archivos y configurar dos Variables de entorno de Windows. Puede parecer complicado, pero es bastante simple, y que veremos a continuación.

Se descargó un archivo ZIP, con múltiples archivos comprimidos.
Creamos un directorio manualmente como 'C:\OracleInstantClient\'. Luego extraemos los archivos del ZIP en esta carpeta

Configuramos las variables de entorno. PATH y TNS_ADMIN.

Variable PATH:
Si esta variable no existe, simplemente haga clic en el botón 'Nuevo' (1), el grupo de variables de entorno.

Así que en nuestro caso que esta variable ya existía con unas instrucciones de Windows, lo que vamos a hacer es modificarlo mediante la inserción de un 'punto y coma' y nuestra nueva instrucción al final. En este caso, a introducir en la variable PATH la ruta o ubicación de nuestro cliente instantánea: 'C:\OracleInstantClient\'. Luego, seleccione la variable PATH (2) y haga clic en el botón 'Editar' (3).



## Instalación del Toad

1.- Nos bajamos el instant client de la web de Oracle.  
*Importante: Aunque se tenga Windows de 64bit se debe descargar el cliente de 32bit*

Debe tener el Cliente de Oracle antes de instalar el Toad.
http://www.telecomhall.com/Data/Sites/3/siteimages/tips/053/tips_053_i.jpg


## Configuración 

ODAC: Oracle Data Access Components

Una alternativa al SQL Developer que ofrece Oracle de manera gratuita es el Toad el cual necesita el cliente de Oracle.

Herramientas de Bases de Datos
+ Tora
+ DbVisualizer
+ SQuirreL SQL
+ Oracle SQL Developer
+ PL/SQL Developer
+ Orbada
+ SQLPal
+ Toad
+ Data Visualization
+ SQL Maestro

## Referencias

Manual de Instalación de Oracle Instant Client y Toad:  
<http://www.telecomhall.com/es/usando-toad-como-la-mejor-herramienta-libre-de-gestion-de-base-de-datos.aspx>

Oracle JET
toolkit JavaScript de Oracle para desarrollo Front e Híbrido.