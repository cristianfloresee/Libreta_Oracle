<h1 align="center">
    Instalación de Oracle Rest Data Service
</h1>


ORDS facilita el desarrollo de interfaces REST modernas para datos relacionales en Oracle Database, Oracle Database 12c JSON Document Store y Oracle NoSQL Database. 


https://4.bp.blogspot.com/-SB3FpGzHueg/Vz45LQ_lLdI/AAAAAAAAuJ4/ExVTxOPAo5ITZcl4DG-uIwytbX5a9ACVwCLcB/s1600/Untitled.png



# 1. Sobre Oracle Rest Data Service

El papel de ORDS es fundamental, ya que permitirá tener una capa REST de la lógica de la base de datos y poder reutilizar las reglas y el modelo desde diferentes frameworks.

Aunque la creación de servicios REST con ORDS se puede hacer por línea de comandos, si lo conectamos desde SQL Developer podemos crear los servicios de una manera muy cómoda.

# 2. Descarga e Instalación de Oracle Rest Data Service

Existen dos formas de instalar el ORDS:

## Primera Forma - Línea de Comandos:

+ Instale un servidor (Para este ejemplo usaremos Apache Tomcat):  
<http://tomcat.apache.org/download-70.cgi>

+ Descargue ORDS:  
<http://www.oracle.com/technetwork/developer-tools/rest-data-services/downloads/index.html>

+ Estando en el directorio del archivo ZIP extraído, ejecute el siguiente comando para instalar el ORDS:  
```
java -jar ords.war
```
+ Luego proporcione la información de la Base de Datos incluyendo un nombre de usuario y contraseña de SYSDBA. Esto es necesario para que ORDS instale el esquema necesario y los paquetes PL/SQL.

<h2 align="center"> [---En Construcción---] </h2>

## Segunda Forma - SQL Developer (Recomendada):

Oracle SQL Developer le permite administrar Oracle REST Data Services utilizando una interfaz gráfica de usuario.

Con esta interfaz gráfica de usuario, puede actualizar las conexiones de base de datos, JDBC, URL, RESTful, seguridad (procedimientos permitidos, procedimientos bloqueados, función de validación y escaneo de virus), caché, procedimientos de pre / post procesamiento, entorno y configuración de Excel. Oracle SQL Developer también proporciona informes estadísticos, informes de errores y registro.

+ Descargar Oracle SQL Developer:  
<http://www.oracle.com/technetwork/developer-tools/sql-developer/downloads/index.html>

+ Ejecutamos la aplicación:  

<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517442306/sshot-199_zsjahm.png">

+ Aparecerá la siguiente ventana de la aplicación:  

<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517442555/sshot-1_y5g2jt.png">

+ Realizamos la Conexión a la Base de Datos:  

<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517929059/sshot-4_degnwx.png">

+ Instalamos ORDS a través de Oracle SQL Developer:  

<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517442943/sshot-2_mais6e.png">

+ Seleccionamos la ubicación del ORDS y la ruta donde se guardará la configuración (ruta de configuración opcional):  

<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517448934/sshot-3_m62sdw.png">

+ Seleccionamos la conexión:

<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517929067/sshot-6_knd2jt.png">

<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517929847/sshot-7_isxxga.png">
<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517929856/sshot-8_otlktk.png">
<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517929856/sshot-9_p0wgqw.png">
<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517929856/sshot-10_nzfmfz.png">
<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517929857/sshot-11_mjemkk.png">
<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517929856/sshot-12_nttbgl.png">
<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517929857/sshot-13_zrgt8w.png">
<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517929856/sshot-14_fcdtgk.png">
<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517929857/sshot-15_marebr.png">
<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517929857/sshot-16_ac7ddq.png">
<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517929857/sshot-17_jxiroh.png">
<img src="http://res.cloudinary.com/dwj4kbnam/image/upload/v1517929857/sshot-18_wzsr1c.png">

# 3. Creación de Servicios de Datos REST desde SQL Developer

+ Para crear una consulta simple basada en un esquema y una tabla existentes, primero debe habilitar el esquema para los servicios REST y luego habilitar la tabla.

+ Para habilitar el esquema, establezca una conexión con SQL Developer. Haga clic con el botón derecho sobre el esquema y seleccione Servicios REST, habilite los servicios REST.

# 4. Otras características

+ Es compatible con Weblogic, Tomcat, Glassfish y también como una aplicación independiente que ejecuta Jetty en modo incrustado.



# 5. Referencias

<https://www.toadworld.com/platforms/oracle/w/wiki/11419.getting-started-with-oracle-rest-data-services>