# 📦 Entrega 2 – Integración Continua y Despliegue Continuo (CI/CD)

## 🎯 Descripción General

En esta segunda entrega, el objetivo es incorporar una herramienta que facilite el proceso de Integración Continua y Despliegue Continuo (CI/CD) para la aplicación desarrollada en la Entrega 1.

---

## 🧩 1. Problema a Resolver

Debemos llevar nuestro proyecto desarrollado en la entrega n°1 a un sistema de Integraión Continua / Despliegue Continuo (CI/CD). Debemos considerar dos elementos clave:

1. **Implementación del sistema CI/CD**.
2. **Mejoras en la aplicación**: Requerimientos pendientes de la entrega anterior y compromisos contraido en entrega 1.

---

## 🛠 2. Tareas a Realizar

### 2.1 Implementación del Sistema CI/CD

- Instalación de Jenkins
- Configuración de Jenkins
- Integración con herramientas existentes

### 2.2 Mejoras en la Aplicación

- Desarrollo de dos nuevos requerimientos funcionales 

### 2.3 Procedimientos

- **Ambiente de Jenkins**: Jenkins puede ser instalado en ambiente local, pero idealmente en la Nube.
- **Integración con Slack y GitHub**: Una vez Jenkins Instalado y configurado, integrar a herramientas Slack y Github.
- **Automatización con Pipelines**: Generar Pipeline de CI/CD, programar Jenkins para que ejecute trabajos automáticamente cada vez que se realicen cambios en el repositorio de código fuente (Cambios asociados a los 2 nuevos requerimientos). Esta es una parte clave de CI/CD.

---

## 🔧 3. Herramientas y Soluciones

### 3.1 Jenkins
Es un servidor de automatización de código abierto, proporciona cientos de complementos para respaldar la creación, implementación y automatización de cualquier proyecto-

- **Recursos Adicionales**:
  - [Curso de Jenkins](https://www.jenkins.io/doc/tutorials/)
  - [Libros sobre Jenkins](https://www.jenkins.io/doc/book/)
  - [Instalación de Jenkins en Máquina Virtual](https://www.jenkins.io/doc/book/installing/)

### 3.2 Ngrok
Es un acceso como servicio de API First, agrega conectividad, observabilidad y seguridad a aplicaciones en una sola línea. Ofrece acceso instantáneo a sus aplicaciones en cualquier nube, red privada o dispositivo con autenticación, equilibrio de carga y otros controles críticos.

- [Enlace a Ngrok](https://ngrok.com/)

### 3.3 Otras Herramientas

- También se puede utilizar otras herramientas de CI/CD, como por ejemplo [Azure DevOps](https://azure.microsoft.com/en-us/products/devops) o [Github actions](https://github.com/features/actions).

### 3.4 Integraciones
Se debe realizar integración entre:

- **GitHub y Jenkins**: Github y Jenkins (Ver uso de WebHook en Github y Ngrok en caso de tener Jenkins Local).
- **Jenkins y Slack**.

---

## 🧪 4. Metodología de Trabajo

### 4.1 Metodología
Uso de misma metodología ya utilizda en entrega 1:
- Mismos equipos
- Usar GitFlow para administrar el flujo de trabajo
- Metodologóa Kanban
  - En Jira configurar proyecto "desarrollo de software" > "Kanban"
  - Crear incidencias del proyecto en el tablero
  - Priorizar
  - Agregar un campo de estiación en horas o Story points de cada historia o tarea
  - Manejar tareas y mantener tablero actualizado

### 4.2 Instrucciones de Presentación

> ⚠️ Esta experiencia solo considera entregable, no presentación.

### 4.3 Fecha de Entrega

- Fechas en aula Moodle

### 4.4 Entregables

1. Enlace a código fuente en GitHub, actualización de código en repositorio
2. Cápsula de video autoexplicativo del trabajo realizado, debe contener al menos:
    1. Alcances de la herramienta
    2. Descripción del trabajo realizado
        1. Proyecto
        2. Especificar dependencias entre la herramienta y la aplicación
    3. Uso de Jenkins
    4. Problemas encontrados y soluciones
3. Actualizar documentación: Incluir información de la integraión Jenkins y actualización de aplicación

> **Nota**: Es requisito de la tarea explicar la infraestructura que soporta la aplicación web, y su relación con las pruebas si es pertinente.

---

> ✅ Para preguntas o aclaraciones, usar el foro de la sección correspondiente en aula Moodle.
