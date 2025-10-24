# api-de-reservas-hoteleras

API de Reservas de Hoteles 🏨
Este proyecto es una API RESTful construida con Node.js y Express para la gestión de reservas de hoteles. Fue desarrollada como parte de un bootcamp para demostrar la implementación de operaciones CRUD, filtrado avanzado y documentación de API.

✨ Características Principales
La API permite realizar operaciones CRUD completas y ofrece 6 endpoints de filtrado para una gestión de datos robusta.

Operaciones CRUD
GET /api/reservas: Obtiene una lista de todas las reservas.

POST /api/reservas: Crea una nueva reserva.

GET /api/reservas/:id: Obtiene una reserva específica por su ID.

PUT /api/reservas/:id: Actualiza una reserva existente por su ID.

DELETE /api/reservas/:id: Elimina una reserva por su ID.

⚡ Filtros Avanzados (Query Params)
El endpoint GET /api/reservas soporta los siguientes parámetros de consulta (query params) para filtrar resultados, los cuales se pueden combinar:

?hotel=...: Filtra por el nombre del hotel.

?tipo_habitacion=...: Filtra por tipo de habitación (ej. "doble", "suite").

?estado=...: Filtra por estado (ej. "pendiente", "confirmada").

?num_huespedes=...: Filtra por un número igual o mayor de huéspedes.

?fecha_inicio=...&fecha_fin=...: Filtra por reservas que se solapan (chocan) con un rango de fechas específico.

🛠️ Tecnologías Utilizadas
Node.js: Entorno de ejecución de JavaScript del lado del servidor.

Express: Framework para la construcción de APIs y aplicaciones web.

Dotenv: Para la gestión de variables de entorno.

Swagger (Opcional):

swagger-jsdoc: Para generar la especificación OpenAPI desde comentarios JSDoc.

swagger-ui-express: Para servir la documentación interactiva de la API.

🚀 Instalación y Ejecución
Sigue estos pasos para levantar el proyecto en tu máquina local:

1. descargar el repositorio y ejecutar
Bash

2. Instalar dependencias
Asegúrate de tener Node.js instalado. Luego, ejecuta:

Bash

npm install
3. Configurar variables de entorno
Crea un archivo .env en la raíz del proyecto. Este archivo contendrá el puerto en el que correrá la aplicación.

PORT=3000
4. Iniciar el servidor
Puedes iniciar el servidor en modo estándar o en modo de desarrollo (si tienes nodemon instalado).

Modo estándar:

Bash

node server.js
Modo desarrollo (recomendado):

Bash

nodemon server.js
¡El servidor estará corriendo en http://localhost:3000!

📚 Documentación (Swagger)
Si tienes la configuración opcional de Swagger activada, puedes acceder a la documentación interactiva de la API una vez que el servidor esté corriendo.

Abre tu navegador y visita:

http://localhost:3000/api-docs
