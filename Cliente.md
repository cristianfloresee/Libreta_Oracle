<h1 align="center">
    Instalación del Cliente de Oracle 11g
</h1>

 A continuación veremos como configurar el Oracle Instant Client, evitando la instalación de una base de datos Oracle.

# 1. Instalación del Cliente

Existen dos formas de instalar el ORDS:

## Primera Forma:

+ Descargamos el Cliente de Oracle:  
<http://www.oracle.com/technetwork/database/enterprise-edition/downloads/112010-win64soft-094461.html>


## Segunda Forma - InstantClient (Recomendada): 

Se recomienda instalar Instant Client, ya que podemos ejecutar nuestras aplicaciones (en este caso Toad) sin tener que instalar el cliente estándar de Oracle, que consume mucho más espacio.

*Importante: Aunque se tenga Windows de 64bit se debe descargar el cliente de 32bit*

La 'instalación' del Oracle Instant Client en realidad consiste en copiar unos archivos y configurar dos Variables de entorno de Windows. Puede parecer complicado, pero es bastante simple, y que veremos a continuación.

Se descargó un archivo ZIP, con múltiples archivos comprimidos.
Creamos un directorio manualmente como 'C:\OracleInstantClient\'. Luego extraemos los archivos del ZIP en esta carpeta

Configuramos las variables de entorno. PATH y TNS_ADMIN.

Variable PATH:
Si esta variable no existe, simplemente haga clic en el botón 'Nuevo' (1), el grupo de variables de entorno.

Así que en nuestro caso que esta variable ya existía con unas instrucciones de Windows, lo que vamos a hacer es modificarlo mediante la inserción de un 'punto y coma' y nuestra nueva instrucción al final. En este caso, a introducir en la variable PATH la ruta o ubicación de nuestro cliente instantánea: 'C:\OracleInstantClient\'. Luego, seleccione la variable PATH (2) y haga clic en el botón 'Editar' (3).

# 2. Instalación de ODAC


# 3. Referencias
