
# 📦 Entrega 3 - Pruebas de interfaz con Selenium

## 🎯 Resumen rápido

En esta tercera entrega, el objetivo es sumar pruebas de interfaz (E2E/UI) a la solución construida en Entrega 1 e integrada a CI/CD en Entrega 2, y dejar todo corriendo automáticamente dentro del pipeline.

Al finalizar, el proyecto debe tener:

- Un set de **pruebas E2E/UI** (por defecto Selenium, o alternativa equivalente).
- Esas pruebas integradas al **pipeline de CI/CD**.
- Evidencia clara de ejecución (logs + reportes + fallas visibles) y notificaciones a Slack.

Hemos avanzando de la siguiente forma: 

- Entrega 1: construimos una aplicación (MVP CRUD) y agregamos pruebas automatizadas.
- Entrega 2: incorporamos Jenkins y un pipeline CI/CD.
- Entrega 3: incorporamos pruebas de interfaz usando una herramienta E2E (por defecto Selenium) y las integramos al pipeline.
---

## ❓ 1. El Problema

En la entrega uno (1) generamos una aplicación y la probamos con una herramienta de testing. En la entrega dos (2) sumamos Jenkins al proceso y creamos un Pipeline.

En esta oportunidad, crearemos un conjunto de pruebas en alguna herramienta E2E, por defecto **[Selenium](https://www.selenium.dev/)** y lo integraremos a nuestro Pipeline. 

Si no usaste previamente alguna de las siguientes herramientas, puedes usarla en lugar de Selenium:

1. **[Playwraight](https://playwright.dev/)** enables reliable end-to-end testing for modern web apps.
1. **[Puppeteer](https://pptr.dev/)** is a Node.js library which provides a high-level API to control Chrome/Chromium over the DevTools Protocol. Puppeteer runs in headless mode by default, but can be configured to run in full ("headful") Chrome/Chromium.
1. **[Robot Framework](https://robotframework.org/)** is a generic open source automation framework. It can be used for test automation and robotic process automation (RPA). Robot Framework is supported by Robot Framework Foundation. Many industry-leading companies use the tool in their software development.

Elijas la que elijas, debes cumplir el objetivo: **E2E/UI automatizado + integrado al pipeline + evidencia + notificaciones.**

---

## 📝 2. ¿Qué debo hacer?

### 🕵️‍♂️ 2.1 Elegir herramienta E2E (por defecto Selenium)

**Selenium** es un conjunto de herramientas de código abierto diseñadas para la automatización de navegadores web. Es ampliamente utilizado para realizar pruebas automatizadas de aplicaciones web en diversos navegadores y plataformas. Selenium proporciona una interfaz para interactuar con los elementos de una página web, simular acciones del usuario y verificar el comportamiento de la aplicación.

[Documentación Selenium](https://www.selenium.dev/documentation/)

### 2.2 Definir y automatizar un set de pruebas E2E/UI
**Objetivo:** cubrir escenarios críticos de usuario final.

**Requerimiento mínimo recomendado (para corregir fácil):**
- Al menos **10 pruebas E2E** enfocadas en flujos críticos.

**Escenarios sugeridos (elige los que apliquen a tu app):**
- **CRUD Happy Path:** crear → listar → ver detalle → editar → eliminar.
- **Validaciones / errores:** campos obligatorios, input inválido, mensajes.
- **Búsqueda / filtro** (si existe).
- **Login / permisos** (si aplica).
- **Navegación clave:** acceso a vistas principales sin errores.

> Si algún flujo no existe en tu solución, reemplázalo por uno equivalente y explícalo.

### 2.3 Integrar pruebas de interfaz al CI/CD (Pipeline)
Debes integrar la ejecución de E2E en el pipeline (Jenkins) de Entrega 2.

**Debe ocurrir lo siguiente:**
- Cada vez que haya cambios en el repositorio, el pipeline:
  1) levanta el entorno necesario (app + dependencias)
  2) ejecuta las pruebas E2E
  3) marca el build como **OK / FAIL** según el resultado

**Reglas prácticas (para que funcione en CI):**
- Las pruebas deben poder correr **headless** (sin abrir navegador visible).
- Usar `BASE_URL` por variable de entorno (no hardcodear localhost).
- Si hay DB o datos, definir una estrategia mínima:
  - seed de datos / data fija de prueba / reset entre tests (lo que aplique).

### 2.4 Integraciones (obligatorias)
- Subir scripts de pruebas E2E al repositorio en GitHub.
- Configurar Jenkins para ejecutar automáticamente estas pruebas al detectar cambios en el repo.
- Configurar notificaciones a Slack con el resultado (éxito/falla).

---

## ✅ 3) Definition of Done (DoD) — Checklist de aprobación
Tu Entrega 3 se considera completa si cumple todo esto:

- [ ] Existe un set de pruebas E2E/UI (mínimo recomendado: 5).
- [ ] Las pruebas cubren escenarios críticos (explicados en documentación).
- [ ] Se ejecutan automáticamente en el pipeline de Jenkins.
- [ ] El pipeline falla si falla una prueba E2E.
- [ ] Hay evidencia (logs, reportes y/o screenshots) de la ejecución.
- [ ] Notificaciones a Slack informan estado del job/pipeline.

---
## 📚 4. Metodología

### 🏗️ 4.1 Metodología de trabajo

- Uso de la misma metodología ya utilizada en las entregas 1 y 2:
  - Mismos equipos de trabajo.
  - Usar **GitFlow** para administrar el flujo de trabajo.
  - Continuar con la metodología **Kanban**.
  - Agregar nuevas tareas y priorizarlas.
  - Agregar un campo de estimación en horas o Story Points a cada historia o tarea.
  - Manejar tareas y mantener el tablero actualizado.

### 🎤 4.2 Instrucciones presentación

- Se realizará una presentación en el horario de clases de la fecha señalada, exponiendo los grupos que **NO** expusieron en la presentación 1.

### 📆 4.3 Fechas

- Fechas en aula Moodle

---

## 📦 5) Entregables
1) **Código actualizado en GitHub**
- Incluye pruebas E2E/UI y ajustes al pipeline.

2) **Cápsula de video autoexplicativa** (obligatoria), debe incluir al menos:
- Alcances de la solución implementada.
- Herramienta E2E utilizada (Selenium/otra) y cómo corre.
- Paso a paso del trabajo realizado.
- Integración con pipeline y ejecución automática.
- Problemas encontrados y cómo los solucionaron.

3) **Documento completo** (puede estar en GitHub) que cubra lo mismo que el video:
- Qué hicieron, cómo se ejecuta, evidencia, problemas y soluciones.

---
# 📎 ANEXOS

## Anexo A — Recomendaciones técnicas para E2E (para evitar dolores típicos)
- Usar selectores estables (`data-testid` o equivalentes) en vez de selectores frágiles.
- Guardar evidencia cuando falle un test (screenshot, log, reporte).
- Evitar dependencias externas inestables en E2E (si dependen de APIs externas, mockear o aislar si es posible).
- Mantener tests E2E como “flujos de usuario”, no como unit tests.

---

## Anexo B — Wiki Entrega 3 (qué debe contener)
Crea una página específica en la Wiki con título principal:

## **“Entrega 3”**

**Contenido recomendado (en orden):**
1. **Objetivo de la Entrega 3**
2. **Herramienta E2E elegida**
   - Selenium o alternativa, y por qué
3. **Set de pruebas E2E**
   - listado de casos (nombre + qué valida)
   - escenarios críticos cubiertos
4. **Cómo ejecutar local**
   - prerequisitos (si aplica)
   - comandos/pasos
5. **Integración con CI/CD**
   - dónde está la etapa/job E2E
   - qué gatilla el pipeline (push/PR)
   - variables (ej: `BASE_URL`)
6. **Evidencias**
   - logs del job
   - reportes
   - screenshots en fallos (si aplica)
   - link al build o a la ejecución
7. **Problemas encontrados y soluciones**
8. **Pendientes / mejoras futuras** (opcional, pero recomendado)

---

✅ Para preguntas o aclaraciones, usar el foro de la sección correspondiente en Aula.
