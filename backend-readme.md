# UPBlioteca Backend

Este repositorio contiene el código del backend para UPBlioteca, una plataforma web que permite a estudiantes universitarios compartir y encontrar documentos de estudio.

## Descripción

El backend de UPBlioteca proporciona la API y la lógica del servidor necesarias para soportar las funcionalidades de la aplicación web frontend. Está diseñado para manejar la autenticación de usuarios, el almacenamiento y recuperación de documentos, y otras operaciones cruciales para el funcionamiento de la plataforma.

## Características principales

- 🔐 Autenticación y autorización de usuarios
- 📁 Gestión de documentos (subida, descarga, actualización, eliminación)
- 🔍 API para búsqueda de documentos
- ⭐ Sistema de calificación de documentos
- 👤 Gestión de perfiles de usuario
- 📊 Seguimiento y análisis de descargas

## Tecnologías utilizadas

- Node.js
- Express.js
- MongoDB
- JWT para autenticación
- Multer para manejo de archivos
- Mongoose para modelado de datos
- Bcrypt para encriptación de contraseñas

## Requisitos previos

- Node.js (versión 14 o superior)
- MongoDB
- npm o yarn

## Instalación

1. Clona el repositorio:
   ```
   git clone https://github.com/tu-usuario/upblioteca-backend.git
   cd upblioteca-backend
   ```

2. Instala las dependencias:
   ```
   npm install
   ```

3. Configura las variables de entorno:
   Crea un archivo `.env` en la raíz del proyecto y añade las siguientes variables:
   ```
   PORT=5000
   MONGODB_URI=tu_uri_de_mongodb
   JWT_SECRET=tu_secreto_jwt
   ```

4. Inicia el servidor:
   ```
   npm start
   ```

El servidor debería estar corriendo en `http://localhost:5000`.

## Scripts disponibles

- `npm start`: Inicia el servidor
- `npm run dev`: Inicia el servidor con nodemon para desarrollo
- `npm test`: Ejecuta las pruebas
- `npm run lint`: Ejecuta el linter

## Estructura del proyecto

```
upblioteca-backend/
├── src/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── utils/
│   └── app.js
├── tests/
├── .env
├── .gitignore
├── package.json
└── README.md
```

## API Endpoints

- `POST /api/auth/register`: Registro de usuarios
- `POST /api/auth/login`: Inicio de sesión
- `GET /api/documents`: Obtener lista de documentos
- `POST /api/documents`: Subir un nuevo documento
- `GET /api/documents/:id`: Obtener un documento específico
- `PUT /api/documents/:id`: Actualizar un documento
- `DELETE /api/documents/:id`: Eliminar un documento
- `POST /api/documents/:id/rate`: Calificar un documento

Para una documentación completa de la API, por favor consulta el archivo `API_DOCS.md`.

## Contribuir

1. Haz un fork del proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Haz commit de tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Haz push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo `LICENSE.md` para más detalles.

## Contacto

Email: hrcamilo11@gmail.com
Enlace del proyecto: https://github.com/tu-usuario/upblioteca-backend

## Relacionado

- [UPBlioteca Frontend](https://github.com/hrcamilo11/Notas---Next): Repositorio del frontend de UPBlioteca
