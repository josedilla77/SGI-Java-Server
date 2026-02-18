# SGI - Sistema de Gestión de Incidencias
**Autor:** JOSE LUIS LLAMAS
**Versión:** 1.0

**Enlace:** https://github.com/josedilla77/SGI-Java-Server/tree/main

## 1. Descripción del Proyecto
Esta es una aplicación web backend desarrollada en Java para la 
gestión de errores técnicos. Permite a los usuarios reportar incidencias y 
almacenarlas en una base de datos centralizada.

## 2. Tecnologías Utilizadas
- **Lenguaje:** Java 17
- **Framework:** Spring Boot 4.x
- **Persistencia:** JDBC (Java Database Connectivity)
- **Base de Datos:** MariaDB / MySQL
- **Documentación:** OpenAPI

## 3. Requisitos de Instalación 
Para que este servidor funcione en otro ordenador, se necesita:
1. Tener instalado el **JRE 17** (Java Runtime Environment).
2. Tener acceso a un servidor **MariaDB** con una base de datos 
llamada `sgi_db`.
3. Importar el script SQL de tablas que se encuentra en la carpeta `/sql`.
## 4. Guía de Uso de la API
Una vez arrancado el servidor, podéis acceder a la documentación 
interactiva en:
`http://localhost:8080/swagger-ui/index.html`
### Endpoints principales:
- `GET /api/incidencias`: Recupera el listado completo de incidencias en 
formato JSON.
- `POST /api/incidencias`: Envía una nueva incidencia. (Requiere un 
JSON con `titulo` y `descripcion`).

## 5. Pruebas de Rendimiento
Se han realizado pruebas de estrés con **JMeter**. 
- **Capacidad máxima detectada:** 100 usuarios concurrentes.
- **Tiempo medio de respuesta:** 150ms.

