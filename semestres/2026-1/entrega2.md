# 📦 Entrega 2 – Integración Continua y Despliegue Continuo (CI/CD)

## 🎯 Descripción General

En esta segunda entrega, el objetivo es incorporar una herramienta que facilite el proceso de Integración Continua y Despliegue Continuo (CI/CD) para la aplicación desarrollada en la Entrega 1.

---

## 🧩 1. Problema a Resolver

Debemos llevar nuestro proyecto desarrollado en la entrega n°1 a un sistema de Integraión Continua / Despliegue Continuo (CI/CD). 

Debemos lograr, concretamente:
- **Automatizar el flujo CI/CD**: que Jenkins ejecute un pipeline cada vez que hay cambios en el repo (push/PR) usando webhooks.
- **Integrar el trabajo con GitHub**: que el estado del build/tests quede asociado al commit/PR (verde/rojo), y no dependa de “en mi máquina funciona”.
- **Ejecutar tareas estándar siempre igual**: típicamente build + tests (y si aplica, empaquetado/deploy), sin pasos manuales.
- **Detectar errores temprano**: que falle rápido si algo rompe (compilación, dependencias, tests), antes de seguir avanzando.
- **Dar trazabilidad**: historial de ejecuciones, logs, artefactos/resultados; evidencia clara para la entrega.
- **Notificar al equipo**: con Slack, avisar cuándo el pipeline falla o pasa, para reaccionar rápido.
- **Profesionalizar la infraestructura**: demostrar que el proyecto tiene una base “de industria” para seguir escalando en Entrega 3.

Además, debemos considerar:

1. **Implementación del sistema CI/CD**.
2. **Mejoras en la aplicación**:
   - Nuevos requisitos según prioridades
   - Requisito pendientes de la entrega anterior y compromisos contraido en entrega 1.
   - Pruebas asociadas a las funcionalidades agregadas

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
- Contimnuar con el uso de metodología Kanban

### 4.2 Instrucciones de Presentación

> ⚠️ Esta experiencia solo considera entregable, no presentación.

### 4.3 Fecha de Entrega

- Fechas en aula Moodle

## 📦 5) Entregables

1. Enlace a código fuente en GitHub, actualización de código en repositorio
2. Cápsula de video autoexplicativo del trabajo realizado, debe contener al menos:
    1. Alcances de la herramienta
    2. Descripción del trabajo realizado
        1. Proyecto
        2. Especificar dependencias entre la herramienta y la aplicación
    3. Uso de Jenkins
    4. Problemas encontrados y soluciones
3. Actualizar documentación: Incluir información de la integraión Jenkins y actualización de aplicación. **Ver anexo A**

> **Nota**: Es requisito de la tarea explicar la infraestructura que soporta la aplicación web, y su relación con las pruebas si es pertinente.

> ✅ Para preguntas o aclaraciones, usar el foro de la sección correspondiente en aula Moodle.

---
# 📎 ANEXOS

## Anexo A, Qué debe contener la documentación de la Entrega 2

Contenido recomendado:

1.	Objetivo de la Entrega 2
   -	Qué se busca lograr con CI/CD en este proyecto.

2.	Qué se implementó
  - Lista breve: Jenkins instalado/configurado + integraciones + pipeline + 2 requerimientos.

3.	Arquitectura / Infraestructura (obligatoria)
  -	Dónde corre la app.
  - Dónde corre Jenkins (local o nube).
  -	Cómo se conectan (GitHub WebHook, Ngrok si aplica, Slack).
  
4.	Pipeline CI/CD
  - Qué gatilla el pipeline (push/PR/branch).
  -	Qué etapas tiene (ej: build, tests, deploy si aplica).
  -	Evidencias: logs, screenshots, badge, etc.

5.	Integraciones
  -	GitHub ↔ Jenkins (cómo lo lograron).
  -	Jenkins ↔ Slack (qué notifica y cuándo).

6.	Cómo ejecutar 
  -	Cómo levantar Jenkins (o link).
  -	Cómo correr pipeline manual (si se puede).
  -	Cómo probar que el webhook funciona (pasos simples).

7.	Mejoras en la aplicación
  -	Nuevos requerimientos (qué son, dónde están).

8.	Pruebas y relación con CI
   -	Qué pruebas se ejecutan en CI.
   -	Resultado esperado (verde/rojo).

9.	Problemas encontrados y soluciones
   - “Qué falló” + “Cómo lo arreglamos”.

10.	Evidencia
   - Capturas/logs relevantes.

--- 
