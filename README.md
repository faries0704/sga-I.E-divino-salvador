# SIS-GPA-001  
# Sistema de Gestión de Procesos Académicos

<p align="center">
<img src="https://img.shields.io/badge/Laravel-Framework-red" alt="Laravel">
<img src="https://img.shields.io/badge/PHP-8.x-blue" alt="PHP">
<img src="https://img.shields.io/badge/MySQL-Database-orange" alt="MySQL">
<img src="https://img.shields.io/badge/Scrum-Metodolog%C3%ADa-green" alt="Scrum">
<img src="https://img.shields.io/badge/GitFlow-Control%20de%20Versiones-purple" alt="GitFlow">
</p>


# Descripción del Proyecto

El **Sistema de Gestión de Procesos Académicos SIS-GPA-001** es una plataforma web desarrollada para la **Institución Educativa Particular "Divino Salvador"**, ubicada en la provincia de Chachapoyas, región Amazonas - Perú.

El sistema tiene como propósito modernizar y optimizar la gestión académica y administrativa mediante la centralización de información, automatización de procesos y mejora en la comunicación entre los diferentes actores de la comunidad educativa.

La solución permite reemplazar procesos manuales basados en documentos físicos, archivos de Excel y registros descentralizados por una plataforma web segura, organizada y accesible.

El proyecto fue desarrollado aplicando buenas prácticas de ingeniería de software mediante:

- Arquitectura Modelo-Vista-Controlador (MVC).
- Framework Laravel.
- Base de datos relacional MySQL.
- Metodología ágil Scrum.
- Control de versiones GitFlow.
- Revisión de código mediante Pull Requests.
- Despliegue continuo mediante Railway.


---

# Objetivo del Sistema

Desarrollar e implementar un sistema web que permita gestionar y centralizar los procesos académicos y administrativos de la Institución Educativa Particular "Divino Salvador", automatizando actividades como registro de estudiantes, asistencia, evaluaciones, comunicación institucional y generación de información académica.

El sistema busca mejorar la eficiencia operativa, reducir errores humanos, proteger la información institucional y facilitar la toma de decisiones mediante información organizada y disponible.


---

# Problemática Identificada

Antes de la implementación del SIS-GPA-001, la institución educativa presentaba dificultades debido al manejo descentralizado de información mediante herramientas tradicionales.

Los principales problemas identificados fueron:

- Uso de archivos Excel independientes para registros académicos.
- Falta de una base de datos centralizada.
- Retrasos en la consolidación de calificaciones.
- Dificultad para realizar seguimiento de asistencia.
- Falta de acceso inmediato a información académica.
- Riesgo de pérdida, duplicidad o modificación no autorizada de información.
- Comunicación limitada entre docentes, estudiantes y apoderados.

Ante esta situación, se desarrolló una plataforma web integrada que permite administrar los procesos académicos de forma eficiente, segura y escalable.


---

# Funcionalidades Principales


## Gestión de Usuarios y Seguridad

El sistema implementa autenticación y control de acceso basado en roles (RBAC), permitiendo administrar los permisos según las funciones de cada usuario.

Características:

- Registro y administración de usuarios.
- Inicio de sesión seguro.
- Gestión de roles y permisos.
- Control de acceso basado en responsabilidades.
- Validación de credenciales.
- Protección de información académica.
- Bloqueo temporal después de intentos fallidos de autenticación.


### Roles del Sistema

- Administrador.
- Docente.
- Estudiante.
- Apoderado.


---

# Gestión Académica

Permite administrar los principales procesos educativos:

- Gestión de estudiantes.
- Registro de docentes.
- Administración de cursos.
- Gestión de grados y secciones.
- Control de matrículas.
- Registro de asistencia.
- Registro de calificaciones.
- Evaluación por competencias.
- Consulta del historial académico.


---

# Comunicación Institucional

El sistema facilita la comunicación entre los miembros de la comunidad educativa mediante:

- Publicación de avisos institucionales.
- Comunicación entre docentes y apoderados.
- Difusión de información académica.
- Consulta de comunicados oficiales.


---

# Gestión Administrativa

Incluye funcionalidades orientadas a mejorar los procesos administrativos:

- Generación de reportes académicos.
- Gestión documental.
- Administración de información institucional.
- Procesos de traslado y matrícula.


---

# Arquitectura del Sistema

El sistema está desarrollado utilizando el patrón arquitectónico:

# Modelo-Vista-Controlador (MVC)


## Modelo

Gestiona la información del sistema y la comunicación con la base de datos mediante el ORM Eloquent de Laravel.


## Vista

Responsable de la interfaz gráfica del usuario utilizando:

- Blade Templates.
- HTML5.
- CSS3.
- JavaScript.
- Bootstrap.


## Controlador

Contiene la lógica de negocio y controla la comunicación entre modelos y vistas.


La arquitectura MVC permite:

- Mejor organización del código.
- Mayor facilidad de mantenimiento.
- Separación de responsabilidades.
- Escalabilidad futura.


---

# Tecnologías Utilizadas


## Backend

- PHP 8.x.
- Laravel Framework.


## Frontend

- Blade Templates.
- HTML5.
- CSS3.
- JavaScript.
- Bootstrap.


## Base de Datos

- MySQL.


## Herramientas de Desarrollo

- Visual Studio Code.
- Composer.
- Git.
- GitHub.
- MySQL Workbench.
- phpMyAdmin.


## Gestión del Proyecto

- Scrum.
- Trello.
- Microsoft Project.


## Diseño

- Canva.
- dbdiagram.io.


## Despliegue

- Railway Cloud Platform.


---

# Requisitos del Sistema


Antes de ejecutar el proyecto es necesario contar con:


- PHP 8.x o superior.
- Composer 2.x o superior.
- MySQL 8.x o superior.
- Node.js.
- NPM.
- Git.


---

# Instalación del Proyecto


## 1. Clonar el repositorio

```bash
git clone https://github.com/faries0704/sga-I.E-divino-salvador.git
```


Ingresar al directorio del proyecto:

```bash
cd sga-I.E-divino-salvador
```


---

# 2. Instalar dependencias PHP

Ejecutar:

```bash
composer install
```


---

# 3. Configuración del archivo .env


Copiar el archivo de configuración:

```bash
cp .env.example .env
```


Generar la clave de aplicación:

```bash
php artisan key:generate
```


Configurar la conexión con MySQL:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=sga_database
DB_USERNAME=root
DB_PASSWORD=
```


---

# 4. Crear la Base de Datos


Crear la base de datos en MySQL:

```sql
CREATE DATABASE sga_database;
```


---

# 5. Ejecutar Migraciones


Crear las tablas necesarias:

```bash
php artisan migrate
```


Cargar información inicial:

```bash
php artisan db:seed
```


---

# 6. Instalar Dependencias Frontend


Instalar paquetes necesarios:

```bash
npm install
```


Compilar recursos para producción:

```bash
npm run build
```


Para desarrollo:

```bash
npm run dev
```


---

# 7. Ejecutar la Aplicación


Iniciar el servidor Laravel:

```bash
php artisan serve
```


El sistema estará disponible en:


```
http://127.0.0.1:8000
```


---

# Flujo de Desarrollo


El proyecto utiliza GitFlow como estrategia de control de versiones.


Ramas principales:

```
main
develop
feature/*
```

Proceso de integración:

1. Creación de rama feature.
2. Desarrollo de funcionalidad.
3. Commit estructurado.
4. Pull Request.
5. Code Review.
6. Integración a develop.
7. Despliegue final.


---

# Metodología de Desarrollo


El proyecto fue desarrollado bajo la metodología ágil Scrum.


Se utilizaron:

- Product Backlog.
- Sprint Backlog.
- Sprint Planning.
- Daily Scrum.
- Sprint Review.
- Sprint Retrospective.
- Definition of Done (DoD).


El desarrollo fue dividido en cuatro Sprints:


### Sprint 1

Gestión de usuarios y seguridad.


### Sprint 2

Gestión académica:

- Notas.
- Competencias.
- Asistencia.


### Sprint 3

Comunicación institucional.


### Sprint 4

Procesos administrativos y documentación.


---

# Despliegue


El sistema utiliza Railway como plataforma de despliegue en la nube.


Proceso:

1. Integración del repositorio GitHub.
2. Configuración de variables de entorno.
3. Instalación automática de dependencias.
4. Ejecución de migraciones.
5. Publicación del sistema web.


---

# Seguridad Implementada


El sistema incorpora mecanismos de seguridad como:

- Autenticación de usuarios.
- Control de acceso por roles.
- Validación de datos.
- Protección contra accesos no autorizados.
- Gestión segura de credenciales.
- Integridad referencial en base de datos.


---

# Equipo de Desarrollo


## Product Owner

**Nely Vallejos Saavedra**


## Scrum Master

**Rocio Araeli Diaz Mori**


## Supervisor Técnico

**Dino Cesar Carranza Alberca**


## Equipo de Desarrollo

- Dalmer Caruajulca.
- Marcos Huamanta.
- Frans Silva Avellaneda.
- Mijael Ramos.


---

# Licencia

Este proyecto fue desarrollado con fines académicos para la implementación de un sistema web de gestión académica en la Institución Educativa Particular "Divino Salvador".

