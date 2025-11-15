# 🏢 Unidades Residenciales - App Móvil

Aplicación móvil multiplataforma para la gestión integral de unidades residenciales. Facilita la comunicación entre residentes y administradores, reservas de zonas comunes, gestión de PQRS y más.

## 📱 Características Principales

- 🔐 **Autenticación segura** - Login y registro con validación de usuarios
- 🏘️ **Gestión de unidades** - Administración de múltiples conjuntos residenciales
- 📅 **Reservas** - Sistema de reservas para zonas comunes (salón social, piscina, gimnasio)
- 📢 **Noticias y comunicados** - Publicación y visualización de información importante
- 📝 **Sistema PQRS** - Peticiones, Quejas, Reclamos y Sugerencias con seguimiento
- 🔔 **Notificaciones push** - Alertas en tiempo real vía Firebase

## 🚀 Tecnologías

### Frontend
- **Framework**: Flutter 3.24.0
- **Plataformas**: Android & iOS
- **State Management**: Provider / Riverpod (por definir)
- **UI Inspiration**: C.R. Arándanos

### Backend
- **Runtime**: Node.js 18+
- **Framework**: Express.js
- **Base de datos**: MySQL 8.0
- **Autenticación**: JWT
- **Notificaciones**: Firebase Cloud Messaging

### DevOps
- **CI/CD**: GitHub Actions
- **Contenedores**: Docker + Docker Compose
- **Deployment**: Railway / Render / AWS (configurable)

## 📁 Estructura del Proyecto

```
unidades-residenciales/
├── mobile/          # Aplicación Flutter
├── backend/         # API REST Node.js
├── docs/           # Documentación
└── .github/        # Workflows CI/CD
```

## 🛠️ Instalación y Configuración

### Prerrequisitos

- Flutter SDK 3.24.0+
- Node.js 18+
- MySQL 8.0
- Docker (opcional pero recomendado)
- Git

### 1. Clonar el repositorio

```bash
git clone https://github.com/tu-usuario/unidades-residenciales.git
cd unidades-residenciales
```

### 2. Configurar Backend

```bash
cd backend
npm install
cp .env.example .env
# Edita .env con tus credenciales
npm run dev
```

### 3. Configurar App Móvil

```bash
cd mobile
flutter pub get
flutter run
```

### 4. Usar Docker (Recomendado)

```bash
# En la raíz del proyecto
docker-compose up -d
```

## 📖 Documentación

- [📘 Documentación de API](docs/API.md)
- [🗄️ Esquema de Base de Datos](docs/DATABASE.md)
- [🚀 Guía de Despliegue](docs/DEPLOYMENT.md)
- [🏗️ Arquitectura](docs/ARCHITECTURE.md)

## 🧪 Testing

### Tests del Backend
```bash
cd backend
npm test
npm run test:coverage
```

### Tests de Flutter
```bash
cd mobile
flutter test
flutter test --coverage
```

## 📋 Roadmap

### Fase 1 - Diseño (2 semanas)
- [x] Definición de UI/UX en Figma
- [ ] Validación con cliente

### Fase 2 - Autenticación (1 semana)
- [ ] Login/Registro
- [ ] Gestión de roles
- [ ] Recuperación de contraseña

### Fase 3 - Módulos Core (5 semanas)
- [ ] Gestión de unidades residenciales
- [ ] Noticias y comunicados
- [ ] Sistema de reservas
- [ ] PQRS

### Fase 4 - Integración Final (1.5 semanas)
- [ ] Notificaciones push
- [ ] Testing integral
- [ ] Deploy a producción

## 👨‍💻 Desarrollador

**Luis Fernando Soto**
- Proyecto para: Gonzalo
- Inicio: 22 de noviembre de 2025
- Duración estimada: 8-10 semanas

## 📄 Licencia

Este proyecto es privado y confidencial.

## 📞 Soporte

Para reportar bugs o solicitar features, crear un issue en este repositorio.

---

⭐ **Estado del Proyecto**: En desarrollo

🔧 **Última actualización**: Noviembre 2025
