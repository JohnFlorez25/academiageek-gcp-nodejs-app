# Integrando mi App NodeJS con Cloud SQL
   
1. Crear un nuevo proyecto en Google Cloud Platform.
   
2. Inicializar y sincronizar credenciales 
   
   `gcloud init`

3. Clonar el repositorio: 
   
   `git clone https://github.com/JohnFlorez25/academiageek-gcp-nodejs-app.git`

4. Cambiar de directorio 
   
   `cd academiageek-gcp-nodejs-app/3-binary-data`

5. Crear una nueva instancia en CLOUD SQL.
   
6. Descargar el CLOUD SQL proxy:

    `wget https://dl.google.com/cloudsql/cloud_sql_proxy.linux.amd64`

> NOTA: Ejecute el paso 7 y 9 en una nueva terminal para dejar activo el proxy

7. Cambie el nombre del proxy para usar el nombre de archivo estándar:

    `mv cloud_sql_proxy.linux.amd64 cloud_sql_proxy`

8. Haga que el proxy sea ejecutable:

    `chmod +x cloud_sql_proxy`

9. Ejecute lo siguiente para iniciar el proxy de Cloud SQL y reemplace [YOUR_INSTANCE_CONNECTION_NAME] con el valor de connectionName:

    `./cloud_sql_proxy -dir=/cloudsql \
                  -instances="[YOUR_INSTANCE_CONNECTION_NAME]"`

10. Crear un nuevo bucket haciendo uso del servicio de STORAGE y colocar el nombre del bucket en el archivo de configuración 

> NOTA: recuerde hacer el bucket público para poder acceder a las imágenes

11.  Ejecutar la aplicación 

    `npm start`

12.  Mirar la app en la siguiente ruta 
    
    `http://localhost:8080`

13. Parar la aplicación presionando Ctrl+C.

14. Deplegar la app: 
    
    `gcloud app deploy`

15. Obtener la url donde está desplegada la aplicación:
    
   `gcloud app browse`