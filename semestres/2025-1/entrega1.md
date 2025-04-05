# 📦 Entrega 1 – INF331: Proyecto de Asignatura

## 🎯 Resumen General

La entrega 1 corresponde a la **primera presentación asociada al proyecto de la asignatura**. En esta etapa se busca construir la base de un ambiente CI/CD con:

1. Un problema claro.
1. Herramientas de apoyo.
1. Una metodología de trabajo definida.

---

## 🧩 1. Problema a Desarrollar

Los problemas son entregados como lo haría un cliente: **pueden estar incompletos o desordenados**. Cada equipo debe escoger **un (1) problema** de la siguiente lista:

- Tema nuevo 1
- Tema nuevo 2
- Tema nuevo 3

> ⚠️ Máximo **3 grupos por tema**.

Aunque los requerimientos son amplios, en esta etapa se debe enfocar en implementar un **CRUD** (Create, Read, Update, Delete) de las funcionalidades principales.

### 1.1 ¿Qué debo desarrollar?

Cada aplicación deberá permitir:

1. Listar elementos
1. Buscar un elemento específico
1. Visualizar el detalle de un elemento
1. Agregar un nuevo elemento
1. Editar un elemento existente
1. Eliminar un elemento

#### Ejemplo: VitaCocina 

1. Listar recetas y consejos
1. Buscar recetas (criterios definidos por el equipo)
1. Visualizar receta en detalle (con imagen)
1. Agregar receta y consejo
1. Editar receta y consejo
1. Eliminar receta

> Si alguno de los casos de uso no aplica a su proyecto, se debe **reemplazar por uno más adecuado**.

---

## 🛠 2. Herramientas, Soluciones y Frameworks

Para realizar las pruebas debe apoyarse en alguno de las herramientas que se listarán a continuación:

### 2.1 Herramientas de Testing Automatizado (seleccionar una):

1. **Puppeteer** is a Node.js library which provides a high-level API to control Chrome/Chromium over the DevTools Protocol. Puppeteer runs in headless mode by default, but can be configured to run in full ("headful") Chrome/Chromium.
1. **Jest** is a delightful JavaScript Testing Framework with a focus on simplicity. It works with projects using: Babel, TypeScript, Node, React, Angular, Vue and more! 
1. **Mocha (Chai)** is a feature-rich JavaScript test framework running on Node.js and in the browser, making asynchronous testing simple and fun. Mocha tests run serially, allowing for flexible and accurate reporting, while mapping uncaught exceptions to the correct test cases.
1. **Jasmine** is a behavior-driven development framework for testing JavaScript code. It does not depend on any other JavaScript frameworks. It does not require a DOM. And it has a clean, obvious syntax so that you can easily write tests.
1. **Enzyme** is a JavaScript Testing utility for React that makes it easier to test your React Components' output. You can also manipulate, traverse, and in some ways simulate runtime given the output. Enzyme's API is meant to be intuitive and flexible by mimicking jQuery's API for DOM manipulation and traversal
1. **Cypress** is a JavaScript testing automation solution used for web automation. It enables teams to create web test automation scripts. This solution aims to enable frontend developers and test automation engineers to write web tests in the de-facto web language that is JavaScript for web test automation.
1. **Robot Framework** is a generic open source automation framework. It can be used for test automation and robotic process automation (RPA). Robot Framework is supported by Robot Framework Foundation. Many industry-leading companies use the tool in their software development.
1. **Katalon** is a modern, comprehensivenquality management platform Deliver world-class digital experiences with an AI-augmented platform that lets you plan, author and execute automated tests.
1. **TestComplete** is a automated UI testing that covers you from device cloud to packaged apps. Ensure the quality of your application without sacrificing speed or agility with an easy-to-use, GUI test automation tool. Our AI-powered object recognition engine and script or scriptless flexibility is unmatched, letting you test every desktop, web, and mobile application with ease. (Solo 15 días de prueba)
1. **Watir** is an open source Ruby library for automating tests. Watir interacts with a browser the same way people do: clicking links, filling out forms and validating text.
1. **Testsigma** is a Intuitive, Feature-rich, Affordable Automated Web UI Testing Tool. Testsigma uses AI to create stable and reliable automated tests faster than ever and to speed-up the executions and maintenance of your automated tests. No coding skills required.
1. **Unit testing framework**, The unittest unit testing framework was originally inspired by JUnit and has a similar flavor as major unit testing frameworks in other languages. It supports test automation, sharing of setup and shutdown code for tests, aggregation of tests into collections, and independence of the tests from the reporting framework.

> La elección debe considerar compatibilidad con las tecnologías del equipo.

**Debes elegir bien, porque la elección que hagas debe permitir cumplir con el objetivo de solicitado para la aplicación y además la elección puede tener impacto en tu aplicación, es decir algunas de las herramientas listadas son específicas para ciertas tecnologías, por lo tanto si quieres usarla deberás usar determinados lenguajes de programación. Todo lo anterior tiene un impacto en el tiempo de desarrollo de esta presentación.**

### 2.2 Integraciones

- Configurar proyecto en **JIRA**.
- Integrar **GitHub + Slack + JIRA** (pueden usar configuraciones previas).

### 2.3 Plataforma en la Nube

Se sugiere usar [Azure for Students](https://azure.microsoft.com/es-es/free/students/):

- 100 USD en crédito gratuito.
- No requiere tarjeta de crédito.

> 🔍 Una VM básica consume aprox. 30-40 USD al mes si está 100% activa.

> ℹ️ Recomendación: Configurar GitHub Copilot (gratis para estudiantes).

> ⚠️ Apagar los servicios en la nube cuando no se estén utilizando.

---

## 🧪 3. Metodología

### 3.1 Metodología de Trabajo

- Equipos de 4, presentados en aula de asignatura.
- Asignar **roles internos** (incluyendo un líder de equipo).
- Crear organización y repositorio en **GitHub**.
- Usar **GitFlow** para el flujo de trabajo.
- Aplicar **Kanban** con proyecto de tipo "Desarrollo de software" en JIRA.
- Crear ítems en el tablero, priorizarlos y estimarlos (horas o story points).
- Tablero siempre debe estar actualizado.

> Herramientas recomendadas: GitHub + Slack + JIRA.

### 3.2 Instrucciones de Presentación 1

- Inscribir en el foro proyecto (aula Moodle):
  - Tema elegido
  - Herramienta de testing elegida

> ⚠️ Máximo 2 grupos por herramienta de testing.

- Si un equipo quiere utilizar alguna herramienta distinta puede hacerlo, pero debe informar y cumplir con el objetivo de probar la aplicación.
- Declarar supuestos por escrito.
- El diseño gráfico queda a criterio del equipo.
- Preguntas en "foro proyecto en Moodle"

### 3.3 Fechas Relevantes

- Fechas en aula Moodle

---

## 📦4 Entregables
Se deben cosiderar los siguientes entregables:

 1. Repositorio con código fuente en GitHub
 2. Documentación del proyecto
 3. Cápsula de video explicativa
 4. Presentación en clases (si eres seleccionado)

### 4.1 Repositorio con código fuente
1. README de instalación (completo, de acuerdo a definiciones presentadas en aula)
1. Documentación de aplicación
1. Licencia
1. .gitignore, correctamente configurado
1. Estructura de carpeta y archivos, de acuerdo a diseño de software
1. Código de aplicación
1. Cápsula de video explicativa
1. Información de Contacto y Contribución

### 4.2 Documentación (en Markdown en el mismo repo):
Para asegurar una documentación completa y útil en el repositorio de GitHub, es esencial incluir los siguientes elementos:

1. **Resumen del Proyecto**
Una descripción concisa que abarque los objetivos, alcance y propósito del proyecto.

1. **Descripción del Trabajo Realizado**
Un detalle de las actividades llevadas a cabo, destacando las funcionalidades implementadas y los logros alcanzados.

1.**Tecnologías de Aplicación y su Relación con las Pruebas**
Listado de las tecnologías y herramientas utilizadas en el desarrollo, explicando cómo cada una contribuye al proceso de pruebas y aseguramiento de calidad.

1.**Evidencia del Trabajo Realizado**
Incluir capturas de pantalla, fragmentos de código, resultados de pruebas y cualquier otro material que demuestre el progreso y los resultados obtenidos.

1.**Estrategia de Pruebas**
Descripción de la metodología de pruebas adoptada, tipos de pruebas realizadas (unitarias, de integración, etc.), pruebas de Frontend, Backend, herramientas empleadas y cobertura de pruebas.

1.**Supuestos y dependencias**
2.**Listado de condiciones asumidas durante el Desarrollo**
Cualquier suposición hecha que haya influido en las decisiones de diseño o implementación.
2.**Identificación de factores externos que pueden influir en el proyecto**
Dependencias de terceros, limitaciones tecnológicas o cualquier otro factor externo relevante.

Para estructurar y presentar esta documentación de manera efectiva, se recomienda:

- **Archivo README.md**
Este archivo, ubicado en la raíz del repositorio, debe proporcionar una visión general del proyecto, incluyendo el resumen, instrucciones de instalación, uso básico y enlaces a documentación más detallada.​

- **Wiki del proyecto*
Utilizar la wiki de GitHub para documentar en profundidad aspectos específicos del proyecto, como la estrategia de pruebas, supuestos, dependencias y otros detalles técnicos. Las wikis permiten una organización estructurada y son ideales para documentación extensa.​

- **Carpeta de documentación**
Crear un directorio específico dentro del repositorio, por ejemplo, docs, para almacenar documentos adicionales, imágenes, diagramas y cualquier otro material relevante.

### 4.3 El video
Video debe incluir:

1. Alcances de la herramienta
1. Descripción del trabajo realizado
1. Proyecto y dependencias
1. Estrategia de pruebas utilizadas
1. Procedimiento de ejecución de pruebas
1. Resultados y problemas encontrados

### 4.4 Presentación en Clase

1. Se realiza el día de entrega.
1. Orden de presentación al azar.
1. **Máximo 25 minutos por equipo**.
1. Todo el equipo obtiene la misma nota.

---

## 👥 5. Equipos

*SEquipos asignados en aula Moodle: https://aula.usm.cl/course/view.php?id=47173*

---

> ✅ Para preguntas o aclaraciones, usar el foro de la sección correspondiente.

