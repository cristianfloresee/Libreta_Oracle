<h1 align="center">
    Instalación y Configuración de Oracle Rest Data Service
</h1>



ORDS facilita el desarrollo de interfaces REST modernas para datos relacionales en Oracle Database, Oracle Database 12c JSON Document Store y Oracle NoSQL Database. 


https://4.bp.blogspot.com/-SB3FpGzHueg/Vz45LQ_lLdI/AAAAAAAAuJ4/ExVTxOPAo5ITZcl4DG-uIwytbX5a9ACVwCLcB/s1600/Untitled.png


1. Instale el servidor de Apacha Tomcat.

<http://tomcat.apache.org/download-70.cgi>

# 1. Sobre Oracle Rest Data Service

El papel de ORDS es fundamental, ya que permitirá tener una capa REST de la lógica de la base de datos y poder reutilizar las reglas y el modelo desde diferentes frameworks.

Aunque la creación de servicios REST con ORDS se puede hacer por línea de comandos, si lo conectamos desde SQL Developer podemos crear los servicios de una manera muy cómoda.

# 2. Descarga e Instalación de Oracle Rest Data Service

Existen dos formas de instalar el ORDS:

## Primera Forma:

+ Descargue ORDS:  
<http://www.oracle.com/technetwork/developer-tools/rest-data-services/downloads/index.html>

+ Estando en el directorio del archivo ZIP extraído, ejecute el siguiente comando para instalar el ORDS:  
```
java -jar ords.war
```
+ Luego proporcione la información de la Base de Datos incluyendo un nombre de usuario y contraseña de SYSDBA. Esto es necesario para que ORDS instale el esquema necesario y los paquetes PL/SQL.

Instalaremos Apache Tomcat.
<https://www.toadworld.com/platforms/oracle/w/wiki/11419.getting-started-with-oracle-rest-data-services>


## Segunda Forma - SQL Developer (Recomendada):

ORDS se incluye con las instalaciones de Oracle Database y Oracle SQL Developer.

+ Descargar Oracle SQL Developer:  

<http://www.oracle.com/technetwork/developer-tools/sql-developer/downloads/index.html>

+ Ejecutamos la aplicación:  

<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517442306/sshot-199_zsjahm.png">

+ Aparecerá la siguiente ventana de la aplicación:  

<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517442555/sshot-1_y5g2jt.png">

+ Realizamos la Conexión a la Base de Datos:  

+ Instalamos ORDS a través de Oracle SQL Developer:  

<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517442943/sshot-2_mais6e.png">

+ Seleccionamos la ubicación del ORDS y la ruta donde se guardará la configuración (ruta de configuración opcional).  

<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517448934/sshot-3_m62sdw.png">

# 3. Creación de Servicios de Datos REST desde SQL Developer

+ Para crear una consulta simple basada en un esquema y una tabla existentes, primero debe habilitar el esquema para los servicios REST y luego habilitar la tabla.

+ Para habilitar el esquema, establezca una conexión con SQL Developer. Haga clic con el botón derecho sobre el esquema y seleccione Servicios REST, habilite los servicios REST.

# 4. Otras características

+ Es compatible con Weblogic, Tomcat, Glassfish y también como una aplicación independiente que ejecuta Jetty en modo incrustado.



# 5. Referencias

<https://www.toadworld.com/platforms/oracle/w/wiki/11419.getting-started-with-oracle-rest-data-services>