# Mi primer hola mundo en App Engine

Esta carpeta contiene un ejemplo de código de una pequeña aplicación desplegada en App Engine


# Instrucciones de despliegue

1. Instalar Node.js.
   
2. Instalar git.
   
3. Crear un nuevo proyecto en Google Cloud Platform.
   
4. Inicializar y sincronizar credenciales 
   
   `gcloud init`

5. Clonar el repositorio: 
   
   `git clone https://github.com/JohnFlorez25/academiageek-gcp-nodejs-app.git`

6. Cambiar de directorio 
   
   `cd academiageek-gcp-nodejs-app/1-hello-world`

7. Instalar las depedencias: 
   
   `npm install`
   
8.  Ejecutar la aplicación 

    `npm start`

9.  Mirar la app en la siguiente ruta 
    
    `http://localhost:8080`

10. Parar la aplicación presionando Ctrl+C.
    
11. Deplegar la app: 
    
    `gcloud app deploy`

12. Obtener la url donde está desplegada la aplicación:
    
   `gcloud app browse`

> NOTA: se recomienda eliminar el proyecto para asegurarse de eliminar completamente la App Engine de prueba