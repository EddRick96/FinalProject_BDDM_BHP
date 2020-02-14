# ESCUELA POLITÉCNICA NACIONAL
  Proyecto Final de BDD Multidimensional
  
  Facultad:  ESFOT


Integrantes:

  - Bolaños Erick
  - Heredia Alfonso
  - Pizarra Jhonathan

Descripción:
El presente proyecto abarca todo lo aprendido durante el semestre 2019B de la materia Base de datos Multidimensaional, se tiene por objetivos:
1) Diseñar una arquitectura de Data Lake en la cual tenga el insumo de datos de al menos las siguientes fuentes:

  - Dos bases de datos SQL (Ejemplo: MySQL, SQL-Server, Postgres, Oracle, etc)
  - Dos bases de datos NoSQL(CouchDB, MondoDB, Cassandra, Neo4j, Riak, Redis, etc) 
  - Dos fuentes de Internet (facebook, twitter, webscrapping, etc)
    
2) Como concentrador de datos debe utilizar elasticsearch y con datos actualizados, realizar un caso de estudio para las siguientes temáticas:
    1. Tráfico vehicular en las 5 principales ciudades del Ecuador.
    2. Eventos deportivos en los principales estadios de Ecuador.
    3. Pulso político en 5 ciudades de Ecuador.
    4. Top 10 twitteros en 5 ciudades de Ecuador.
    5. Top 10 quejas en el Ecuador.
    6. Actividades y hobbies.
    7. Conciertos y eventos públicos.
    8. Tema definido por el estudiante.
    9. Restaurantes y sitios de esparcimiento.
    10. Eventos o noticias mundiales.
    
 3) Recopilación de información (se puede realizar con geolocalización o con filtro depalabras).
    * Si se utiliza geolocalización se deberá subdividir la región. 
    * Si se utiliza filtro de palabras se recomienda usar varias palabras por script.
    - Se debe crear la indexación en al menos 2 nodos. (debe crear un clúster)

 4) Visualización: Se creará una página web en la cual se insertará un dashboard (puede ser de kibana o google charts)
Cada caso de estudio debe tener su propio dashboard y de todo el proyecto al menos una visualización debe tener geolocalización.

Entregables:

  1.- Informe (pdf, IEEE doble columna)
El informe ha de contener:
  - Definición del caso de estudio.
  - Objetivos Generales y específicos.  
  - Descripción del equipo de trabajo y actividades realizadas por cada uno.
  - Cronograma de actividades.
- Asignación de actividades a cada miembro de equipo.
- Recurso y herramientas utilizadas.
- Arquitectura de la solución.
- Extracción de datos.
- Análisis de información.
- Visualización de información.
- Resultados obtenidos.
- Conclusiones y Recomendaciones.
- Desafíos y problemas encontrados.
- Link de github del proyecto.


2.- Presentación del proyecto (ppt, pdf o prezi)
  
  - La presentación se realizará por cada miembro del equipo. Su duración será de 30 minutos y ha de contener los elementos mencionados en el informe.


3.- Bases de datos unificadas
  - Se debe crear un archivo unificado (“nombredelproyecto.couch”, “carpeta_indices_de_es.ziip”, etc) de la base de datos recopilada 
durante el desarrollo del proyecto, 
  - Este archivo se lo debe entregar en uno o varios dvd´s.

4.- Scripts: Se proporcionará los links de github donde se encuentran los scripts de

- Cosecha
- Transformación de datos
- MapReduce
- Creación de índices
- Creación de mapping
- Logstash, etc


5.- Video explicativo del proceso completo subido a Youtube [Video](https://www.youtube.com/playlist?list=PL0UqIFf7qfAZx9UhZOhJhy0zEDSUAros6)
##
## Guia del proyecto
Para este proyecto es necesario tener instalado:
* [Cerebro](https://subscription.packtpub.com/book/big_data_and_business_intelligence/9781786465580/12/ch12lvl1sec144/installing-and-using-cerebro)
* [Elasticsearch](https://www.elastic.co/es/downloads/elasticsearch)
* [Logstash](https://www.elastic.co/es/downloads/logstash)
* [Kibana](https://www.elastic.co/es/downloads/kibana)
## Uso de Cerebro, Elasticsearch,  Kibana
Una vez descargado los archivos: 
* Descomprimir (Se recomienda crear una carpteta para descomprimir todos los archivos)
* Ir a través de la línea de comandos (Teclas: Windows + R => escribir cmd => clic enter.)  
```shell
cd "Ruta donde se descomprimieron los archivos"
cd "Nombre de la carpeta"/bin         //Ejecutar el comando correspondiente (elasticsearch, cerebro, kibana)
elasticsearch         //clic enter
```
### Ingresar en el siguiente rden para usar los archivos
* Elasticsearch: `http://localhost:9200`
Copiar el enlace de elasticsearch en cerebro.
* Cerebro: `http://localhost:9000`
* Kibana: `http://localhost:5601`
*Para esto debera ya tener uso de las diferentes bases de datos sean relacionales o no*
## Uso de la carpeta conf
Para usar el archivo conf de aqui primero descargar [Logstash](https://www.elastic.co/es/downloads/logstash) para esto se recomienda una vez descargado, descomprimir el archivo en una ruta donde las carpetas anteriores no tengan espacios o signos especiales en el nombre de sus carpetas.


Nota: logstash no cuenta con un archivo .conf en su carpeta bin para lo cual debe: 
* Crear un archivo .txt.
* Seleccionar en guardar como...
* Poner en nombre del archivo (nombre).conf 
* Cambiar de tipo de archivo .txt a todos los archivos
* Guardar en la carpeta bin de logstash.
*Seguir la guia que esta dentro de la carpeta conf.*
Lista de plugins tanto de [input](https://www.elastic.co/guide/en/logstash/current/input-plugins.html) como de [output](https://www.elastic.co/guide/en/logstash/current/output-plugins.html) que posee logstash.
Luego:
```shell
cd "Ruta donde se descomprimieron los archivos"
cd "Nombre de la carpeta"/bin         //Ejecutar el comando correspondiente (elasticsearch, cerebro, kibana)
logstash-plugin list        //comando para comprobar los plugin instalados
logstash -f (nombre del archivo .conf).conf         //clic enter
```

