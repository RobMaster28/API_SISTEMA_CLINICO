# 🏥 CLÍNICA JESÚS DEL NORTE

**Marzo – Julio 2025**

Este proyecto es una API desarrollada para la gestión integral de una clínica. Ofrece funcionalidades para administrar:

- Pacientes
- Doctores
- Citas médicas
- Atenciones
- Medicamentos
- Recetas
- Generación de boletas

## 🚀 Tecnologías utilizadas

### Lenguajes
- Java 8+

### Frameworks y Librerías
- **Spring Boot**: para el desarrollo del backend
  - Spring MVC
  - Spring Data JPA
  - Spring Security

### Herramientas
- Git (control de versiones)
- Swagger (documentación de la API)
- Postman (pruebas de endpoints)

### En aprendizaje
- Gestión de bases de datos relacionales con **MySQL**

## 🛠️ Funcionalidades clave

- Autenticación y autorización de usuarios
- CRUD de pacientes y doctores
- Agenda médica y gestión de citas
- Registro de atenciones y generación de recetas
- Facturación médica mediante boletas electrónicas

## 📌 Estado del proyecto

Proyecto en desarrollo. Actualmente se trabaja en:
- Integración completa con la base de datos
- Mejoras en seguridad con Spring Security
- Optimización de las interfaces gráficas y endpoints REST

## 🔧 Configuración del entorno


```
# ========== CONFIGURACIÓN GENERAL ==========
# Nombre de la aplicación
spring.application.name=clinic_system

# Ruta base de la API (se recomienda no modificar)
server.servlet.context-path=/system_clinic/api/v0.1/

# Puerto donde se ejecutará la aplicación
server.port=8080

# ========== CONFIGURACIÓN DE BASE DE DATOS ==========
# URL de conexión a la base de datos (modifica el gestor, puerto y nombre de BD)
spring.datasource.url=jdbc:mysql://localhost:3306/NOMBRE_BD?createDatabaseIfNotExist=true

# Usuario de la base de datos (modificar según tus credenciales)
spring.datasource.username=TU_USUARIO

# Contraseña de la base de datos
spring.datasource.password=TU_CONTRASEÑA

# Mostrar las consultas SQL en consola (opcional para debug)
spring.jpa.show-sql=true

# Habilita la generación automática de tablas
spring.jpa.generate-ddl=true

# Define el comportamiento de Hibernate con el esquema de BD
# Opciones: none | validate | update | create | create-drop
spring.jpa.hibernate.ddl-auto=update

# ========== CONFIGURACIÓN DE SWAGGER ==========
# Habilita la documentación OpenAPI
springdoc.api-docs.enabled=true
springdoc.swagger-ui.enabled=true

# ========== CONFIGURACIÓN DE JWT ==========
# Clave secreta para generar tokens (puedes generar una propia)
jwt-secret-word=TU_CLAVE_SECRETA_AQUI

# Tiempo de expiración del token en segundos (10 horas por defecto)
jwt-seconds=36000

# ========== CONFIGURACIÓN DE PAGINACIÓN ==========
# Tamaño de página por defecto en endpoints
page-size=2

# Tamaño de paginación específico para citas
appointment-size=5
appointment-doctor-size=5
appointment-patient-size=5
```
