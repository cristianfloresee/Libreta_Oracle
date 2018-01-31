facilita el desarrollo de interfaces REST modernas para datos relacionales en Oracle Database, Oracle Database 12c JSON Document Store y Oracle NoSQL Database. 
Una aplicación de Java de nivel medio, ORDS asigna verbos HTTP (S) (GET, POST, PUT, DELETE, etc.) a las transacciones de la base de datos y devuelve los resultados formateados con JSON.

+ ORDS se incluye con las instalaciones de Oracle Database y Oracle SQL Developer. Es compatible con Weblogic, Tomcat, Glassfish y también como una aplicación independiente que ejecuta Jetty en modo incrustado.

https://4.bp.blogspot.com/-SB3FpGzHueg/Vz45LQ_lLdI/AAAAAAAAuJ4/ExVTxOPAo5ITZcl4DG-uIwytbX5a9ACVwCLcB/s1600/Untitled.png


1. Instale el servidor de Apacha Tomcat.

* Servidores Soportados por ORDS:
    + Oracle WebLogic
    + GlassFish Server
    + Apache Tomcat

<http://tomcat.apache.org/download-70.cgi>

## 2. Descargue e instale Oracle Rest Data Service

Existen dos formas de instalar el ORDS:

### Primera Forma:

Descargar ORDS:  
<http://www.oracle.com/technetwork/developer-tools/rest-data-services/downloads/index.html>

Instalaremos Apache Tomcat.

El papel de ORDS es fundamental, ya que nos permitirá poder tener una capa REST de la lógica de nuestra base de datos y poder reutilizar reglas y modelo desde diferentes frameworks.

Aunque la creación de servicios REST con ORDS se puede hacer por línea de comandos, si lo conectamos desde SQL Developer podemos crear los servicios de una manera muy cómoda.


<https://www.toadworld.com/platforms/oracle/w/wiki/11419.getting-started-with-oracle-rest-data-services>


### Segunda Forma (Recomendada):

Descargar Oracle SQL Developer:  
<http://www.oracle.com/technetwork/developer-tools/sql-developer/downloads/index.html>

Ejecutamos la aplicación:  
<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517442306/sshot-199_zsjahm.png">

Aparecerá la siguiente ventana de la aplicación:  
<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517442555/sshot-1_y5g2jt.png">

Realizamos la Conexión a la Base de Datos:  
<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517442943/sshot-2_mais6e.png">
