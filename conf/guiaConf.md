Copiar y pegar en el archivo de logstash en la carpeta bin creando un archivo .conf

Parte 1

input {
  couchdb_changes {
    username => "Erick"
    password => "admin123"
    #db   => "noticias_mundiales"
    db => "topcincotwitteros"
    
  }

}

output {

 
      mongodb {
        
        uri => "mongodb+srv://Erick:Admin123@cluster0-yndgh.gcp.mongodb.net/test?retryWrites=true&w=majority"
        collection=>"project"
        database =>"topcincotwitteros"
                
      }
   
}

Parte 2
Descomentar (quitar #) según correspondo para mandar las bases de datos de couchDB a elasticsearch

input {
  couchdb_changes {
    username => "Erick"
    password => "admin123"
    #db   => "noticias_mundiales"
    db => "topcincotwitteros"
    
  }

}

output {
 
      elasticsearch {
        
        index => "topcincotwitteros"
        #index => "noticias_mundiales"
                
      }
   
}
