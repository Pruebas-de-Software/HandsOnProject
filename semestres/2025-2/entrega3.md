
# 📦 Entrega 3 - Pruebas de interfaz con Selenium

## 🎯 Descripción General

Esta presentación tiene por objetivo sumar pruebas de interfaz a nuestra solución.
(segunda presentación)

---

## ❓ 1. El Problema

En la entrega uno (1) generamos una aplicación y la probamos con una herramienta de testing. En la entrega dos (2) sumamos Jenkins al proceso y creamos un Pipeline.

En esta oportunidad, crearemos un conjunto de pruebas en alguna herramienta E2E, por defecto **[Selenium](https://www.selenium.dev/)** y lo integraremos a nuestro Pipeline. 

Si no uusaste previamente alguna de las siguientes herramientas, puedes usarla en lugar de Selenium:

1. **[Playwraight](https://playwright.dev/)** enables reliable end-to-end testing for modern web apps.
1. **[Puppeteer](https://pptr.dev/)** is a Node.js library which provides a high-level API to control Chrome/Chromium over the DevTools Protocol. Puppeteer runs in headless mode by default, but can be configured to run in full ("headful") Chrome/Chromium.
1. **[Robot Framework](https://robotframework.org/)** is a generic open source automation framework. It can be used for test automation and robotic process automation (RPA). Robot Framework is supported by Robot Framework Foundation. Many industry-leading companies use the tool in their software development.

---

## 📝 2. ¿Qué debo hacer?

### 🕵️‍♂️ 2.1 Selenium

**Selenium** es un conjunto de herramientas de código abierto diseñadas para la automatización de navegadores web. Es ampliamente utilizado para realizar pruebas automatizadas de aplicaciones web en diversos navegadores y plataformas. Selenium proporciona una interfaz para interactuar con los elementos de una página web, simular acciones del usuario y verificar el comportamiento de la aplicación.

[Documentación Selenium](https://www.selenium.dev/documentation/)

### 🔗 2.2 Incorporar pruebas de interfaz al sistema CI/CD

- **Preparar un set de pruebas con Selenium:**
  - Implementar un conjunto de pruebas de interfaz utilizando Selenium para garantizar la calidad y funcionalidad de la aplicación web.
  - Asegurar que las pruebas aborden escenarios críticos.

- **Integrar la ejecución de las pruebas al Pipeline desarrollado para la presentación 2:**
  - Ejecutar el Pipeline en el proceso de integración continua.

### 🔧 2.3 Integraciones

- **Añadir los scripts de prueba de Selenium al repositorio GitHub.**
- **Configurar un trabajo en Jenkins para ejecutar automáticamente las pruebas cada vez que se realice una modificación en el código fuente.**
- **Implementar notificaciones en Jenkins para informar sobre el estado de las pruebas vía Slack.**

---

## 📚 3. Metodología

### 🏗️ 3.1 Metodología de trabajo

- Uso de la misma metodología ya utilizada en las entregas 1 y 2:
  - Mismos equipos de trabajo.
  - Usar **GitFlow** para administrar el flujo de trabajo.
  - Continuar con la metodología **Kanban**.
  - Agregar nuevas tareas y priorizarlas.
  - Agregar un campo de estimación en horas o Story Points a cada historia o tarea.
  - Manejar tareas y mantener el tablero actualizado.

### 🎤 3.2 Instrucciones presentación

- Se realizará una presentación en el horario de clases de la fecha señalada, exponiendo los grupos que **NO** expusieron en la presentación 1.

### 📆 3.3 Fechas

- Fechas en aula Moodle

### 📦 3.4 Entregable

- **Enlace al código fuente en GitHub:** Actualización de código en el repositorio.
- **Cápsula de video autoexplicativa del trabajo realizado**, que debe contener al menos:
  - Alcances de la solución implementada.
  - Uso de Selenium.
  - Descripción del trabajo realizado.
  - Proyecto, paso a paso.
  - Problemas encontrados y soluciones.
- **Documento completo como entregable** que responda a los mismos puntos anteriores, el cual puede ser entregado en GitHub.

---

> ✅ Para preguntas o aclaraciones, usar el foro de la sección correspondiente en aula Moodle.
