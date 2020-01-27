# ESCUELA POLITÉCNICA NACIONAL
  Proyecto Final de BDD Multidimensional
  
  Facultad:  ESFOT


Integrantes:

  - Bolaños Erick
  - Barrera Alfonso
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


5.- Video explicativo del proceso completo subido a Youtube 

