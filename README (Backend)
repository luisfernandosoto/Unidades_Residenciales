# 🔧 Backend API - Unidades Residenciales

API REST para la gestión de unidades residenciales construida con Node.js y Express.

## 🚀 Inicio Rápido

### Instalación

```bash
npm install
```

### Configuración

```bash
cp .env.example .env
# Edita el archivo .env con tus credenciales
```

### Ejecutar en desarrollo

```bash
npm run dev
```

### Ejecutar en producción

```bash
npm start
```

## 📡 Endpoints Principales

### Autenticación
- `POST /api/v1/auth/register` - Registrar usuario
- `POST /api/v1/auth/login` - Iniciar sesión
- `POST /api/v1/auth/refresh` - Refrescar token
- `POST /api/v1/auth/forgot-password` - Recuperar contraseña
- `POST /api/v1/auth/reset-password` - Restablecer contraseña

### Usuarios
- `GET /api/v1/users/:id` - Obtener usuario
- `PUT /api/v1/users/:id` - Actualizar usuario
- `DELETE /api/v1/users/:id` - Eliminar usuario

### Unidades Residenciales
- `GET /api/v1/units` - Listar unidades
- `GET /api/v1/units/:id` - Obtener unidad
- `POST /api/v1/units` - Crear unidad (admin)
- `PUT /api/v1/units/:id` - Actualizar unidad (admin)

### Reservas
- `GET /api/v1/reservations` - Listar reservas
- `POST /api/v1/reservations` - Crear reserva
- `PUT /api/v1/reservations/:id` - Actualizar reserva
- `DELETE /api/v1/reservations/:id` - Cancelar reserva

### Noticias
- `GET /api/v1/news` - Listar noticias
- `GET /api/v1/news/:id` - Obtener noticia
- `POST /api/v1/news` - Crear noticia (admin)
- `PUT /api/v1/news/:id` - Actualizar noticia (admin)
- `DELETE /api/v1/news/:id` - Eliminar noticia (admin)

### PQRS
- `GET /api/v1/pqrs` - Listar solicitudes
- `GET /api/v1/pqrs/:id` - Obtener solicitud
- `POST /api/v1/pqrs` - Crear solicitud
- `PUT /api/v1/pqrs/:id` - Actualizar estado (admin)

## 🗄️ Base de Datos

### Ejecutar migraciones

```bash
npm run migrate
```

### Ejecutar seeds (datos de prueba)

```bash
npm run seed
```

### Crear nueva migración

```bash
npm run migrate:create nombre_migracion
```

## 🧪 Testing

### Ejecutar todos los tests

```bash
npm test
```

### Ejecutar tests con coverage

```bash
npm run test:coverage
```

### Ejecutar tests en modo watch

```bash
npm run test:watch
```

## 🐳 Docker

### Construir imagen

```bash
docker build -t unidades-residenciales-api .
```

### Ejecutar con Docker Compose

```bash
docker-compose up -d
```

## 📦 Scripts Disponibles

```json
{
  "start": "node server.js",
  "dev": "nodemon server.js",
  "test": "jest",
  "test:watch": "jest --watch",
  "test:coverage": "jest --coverage",
  "lint": "eslint .",
  "lint:fix": "eslint . --fix",
  "migrate": "node database/migrate.js",
  "seed": "node database/seed.js"
}
```

## 🔒 Seguridad

- Contraseñas encriptadas con bcrypt
- Autenticación con JWT
- Rate limiting implementado
- CORS configurado
- Validación de inputs
- SQL injection protection

## 📊 Monitoreo

Logs disponibles en:
- Consola (desarrollo)
- Archivo `logs/app.log` (producción)

## 🌐 Variables de Entorno

Ver archivo `.env.example` para todas las variables requeridas.

## 🤝 Contribución

1. Crea una rama feature: `git checkout -b feature/nueva-funcionalidad`
2. Commit tus cambios: `git commit -m 'Agrega nueva funcionalidad'`
3. Push a la rama: `git push origin feature/nueva-funcionalidad`
4. Crea un Pull Request

## 📄 Licencia

Privado y confidencial.
