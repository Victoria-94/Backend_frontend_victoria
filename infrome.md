# Practica servidor web
## 1. Titulo
Despliege de Backend-frontend
## 2. Tiempo de duración
8 horas 
## 3. Fundamentos:
 Servicio de Base de Datos:
El uso de contenedores para servicios de base de datos permite desplegar motores como PostgreSQL o MySQL en entornos aislados, facilitando la configuración, escalabilidad y pruebas reproducibles, sin afectar la instalación del sistema anfitrión.

Construcción de Artefactos:
En el caso del Frontend con React, el proceso de construcción genera artefactos estáticos optimizados (HTML, CSS, JS), que serán servidos desde un contenedor web. Para el Backend, se construye una API REST que entrega datos a través de endpoints definidos.

Creación de Imágenes Docker:
La creación de imágenes Docker permite contenerizar tanto el Frontend como el Backend, asegurando entornos consistentes para el despliegue. Mediante el uso de archivos Dockerfile, se define un entorno autocontenible con las dependencias necesarias para cada servicio.

Orquestación con Docker Compose:
Docker Compose permite definir y gestionar múltiples contenedores (backend, frontend, base de datos) a través de un archivo YAML. Esto facilita el levantamiento de todo el entorno de desarrollo o producción con un único comando.

Manejo de variables de entorno:
El uso de variables de entorno permite parametrizar las configuraciones de la aplicación (por ejemplo, rutas de API, configuración de bases de datos), manteniendo el código desacoplado de valores específicos del entorno y mejorando la seguridad y la portabilidad.

## 4. Conocimientos previos.
   
Para realizar esta practica el estudiante necesita tener claro los siguientes temas:
- Contenedores.
- Puerto de salida.
- Ip.
- Documento docker-compose.yml

## 5. Objetivos a alcanzar

- Configurar contenedores Docker para servicios de base de datos.

- Diseñar un contenedor para el Backend (API REST) que entregue datos en formato JSON.

- Construir y contenerizar un Frontend en React que consuma datos desde el Backend.

- Crear y optimizar archivos Dockerfile para generar imágenes eficientes tanto del Backend como del Frontend.

- Definir y estructurar archivos docker-compose.yml para orquestar el despliegue completo de la aplicación (backend + frontend + base de datos).

## 6. Equipo necesario:
  
- Computador con sistema operativo Windows/Linux
- Plataforma Docker playground o desktop
- Docker hub

## 7. Material de apoyo.
   
- Documentacion de tendencias tecnologicas.
- Docker desktop
- Videos ilustrativos
- Documentacion sobre la configuracion del documento para el despliege de backend.
  
## 8. Procedimiento

Paso 1: Crear la base de datos PostgreSQL y pgAdmin, con los volúmenes y redes correspondientes.


Paso 2: Implementar el Backend en un lenguaje adecuado (por ejemplo, Flask para Python) que exponga un endpoint REST /api/datos.

Paso 3: Construir el Frontend en React que consuma los datos de la API y los visualice en una tabla.

Paso 4: Definir un Dockerfile para el Backend que permita contenerizar el servicio REST.

Paso 5: Definir un Dockerfile para el Frontend que permita contenerizar la aplicación React.

Paso 6: Crear un archivo docker-compose.yml que orqueste el Backend, el Frontend y la base de datos.

Paso 7: Verificar que pgAdmin pueda conectarse a PostgreSQL correctamente.


## 9. Resultados esperados:
    
Después de esta práctica podemos concluir que toda la configuración de las dependencias que requiera la aplicación puede ser centralizada dentro de un mismo archivo docker-compose.yml. Mediante este archivo se definen contenedores para la base de datos, Backend y Frontend, variables de entorno, redes y volúmenes. Además, se comprueba la integración completa entre los componentes, mostrando en el Frontend una tabla con los datos obtenidos desde la API REST.


## 10. Bibliografía
    

Fowler, M. (2010). Patterns of Enterprise Application Architecture. Addison-Wesley.

Whiteley, K. (2017). Using Docker: Developing and Deploying Software with Containers. O’Reilly Media.

Turnbull, J. (2014). The Docker Book: Containerization is the new virtualization. https://www.dockerbook.com

Bass, L., Clements, P., & Kazman, R. (2012). Software architecture in practice (3rd ed.). Addison-Wesley.


audio:

<audio controls>
  <source src="media/nota.ogg" type="audio/ogg">
 
</audio>
