# 📱 App Móvil - Unidades Residenciales

Aplicación móvil multiplataforma desarrollada con Flutter para la gestión de unidades residenciales.

## 🚀 Inicio Rápido

### Prerrequisitos

- Flutter SDK 3.24.0 o superior
- Dart 3.0+
- Android Studio / Xcode
- Dispositivo físico o emulador

### Instalación

```bash
# Obtener dependencias
flutter pub get

# Verificar instalación
flutter doctor
```

### Ejecutar en desarrollo

```bash
# Android
flutter run

# iOS (solo en macOS)
flutter run

# Especificar dispositivo
flutter run -d <device_id>
```

### Compilar para producción

```bash
# Android APK
flutter build apk --release

# Android App Bundle (Google Play)
flutter build appbundle --release

# iOS (requiere certificados)
flutter build ios --release
```

## 📁 Estructura del Proyecto

```
lib/
├── main.dart                    # Punto de entrada
├── config/
│   └── app_config.dart         # Configuración global
├── models/                      # Modelos de datos
│   ├── user.dart
│   ├── unit.dart
│   ├── reservation.dart
│   └── pqrs.dart
├── screens/                     # Pantallas de la app
│   ├── auth/
│   ├── home/
│   ├── reservations/
│   ├── news/
│   └── pqrs/
├── widgets/                     # Widgets reutilizables
│   ├── common/
│   └── custom/
├── services/                    # Servicios (API, Storage, etc)
│   ├── api_service.dart
│   ├── auth_service.dart
│   └── notification_service.dart
├── providers/                   # State management
├── utils/                       # Utilidades
│   ├── constants.dart
│   ├── validators.dart
│   └── helpers.dart
└── theme/                       # Temas y estilos
    └── app_theme.dart
```

## 🎨 Pantallas Principales

### Autenticación
- **Login**: Inicio de sesión con email y contraseña
- **Registro**: Registro de nuevos usuarios con validación
- **Recuperar contraseña**: Recuperación vía email

### Home
- Dashboard con accesos rápidos
- Resumen de reservas
- Últimas noticias

### Reservas
- Calendario interactivo
- Lista de zonas disponibles
- Gestión de reservas activas

### Noticias
- Feed de comunicados
- Vista detallada de noticias

### PQRS
- Formulario de solicitudes
- Seguimiento de estado
- Historial

### Perfil
- Información del usuario
- Configuración de la app
- Cerrar sesión

## 🔧 Configuración

### API Base URL

Editar en `lib/config/app_config.dart`:

```dart
class AppConfig {
  static const String apiBaseUrl = 'http://localhost:3000/api/v1';
  static const String apiVersion = 'v1';
}
```

### Firebase (Notificaciones)

1. Descargar `google-services.json` (Android) y `GoogleService-Info.plist` (iOS)
2. Colocar en las carpetas correspondientes:
   - Android: `android/app/`
   - iOS: `ios/Runner/`

## 🧪 Testing

### Tests unitarios

```bash
flutter test
```

### Tests de integración

```bash
flutter test integration_test/
```

### Coverage

```bash
flutter test --coverage
genhtml coverage/lcov.info -o coverage/html
```

## 📦 Dependencias Principales

```yaml
dependencies:
  flutter:
    sdk: flutter
  provider: ^6.0.0           # State management
  http: ^1.1.0               # HTTP requests
  shared_preferences: ^2.2.0 # Local storage
  firebase_messaging: ^14.0.0 # Push notifications
  flutter_local_notifications: ^15.0.0
  intl: ^0.18.0              # Internacionalización
  cached_network_image: ^3.2.0
  image_picker: ^1.0.0
```

## 🎨 Diseño

El diseño está basado en el modelo de la app **C.R. Arándanos** con las siguientes características:

- Material Design 3
- Tema oscuro/claro
- Animaciones fluidas
- UI responsive
- Accesibilidad

## 🔐 Seguridad

- Tokens JWT almacenados de forma segura
- Validación de inputs
- Cifrado de datos sensibles
- Sesiones expiradas automáticamente

## 🌍 Internacionalización

Soporte para:
- 🇪🇸 Español (por defecto)
- 🇺🇸 Inglés (próximamente)

## 📱 Plataformas Soportadas

- ✅ Android 5.0 (API 21) o superior
- ✅ iOS 12.0 o superior

## 🐛 Debug

### Habilitar logs

```dart
// En main.dart
void main() {
  Logger.root.level = Level.ALL;
  runApp(MyApp());
}
```

### Inspeccionar red

Usar Flutter DevTools:
```bash
flutter pub global activate devtools
flutter pub global run devtools
```

## 🚀 Release

### Android

1. Generar keystore:
```bash
keytool -genkey -v -keystore ~/upload-keystore.jks -keyalg RSA -keysize 2048 -validity 10000 -alias upload
```

2. Configurar en `android/key.properties`

3. Build:
```bash
flutter build appbundle --release
```

### iOS

1. Configurar certificados en Xcode
2. Build:
```bash
flutter build ios --release
```

## 📄 Licencia

Privado y confidencial.

## 🤝 Desarrollador

Luis Fernando Soto - 2025