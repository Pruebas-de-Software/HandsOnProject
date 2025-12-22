# 📦 Entrega 1 — Construcción inicial aplicación y pruebas automatizadas

## 🎯 Resumen rápido

Esta entrega es la **primera presentación del proyecto**. El objetivo es construir la base con:

- Un problema claro.
- Herramientas de apoyo.
- Una metodología de trabajo definida.

En esta etapa el foco es implementar las funcionalidades prioritarias de la aplicación, además se debe incluir **CRUD (Create, Read, Update, Delete)** de funcionalidades principales: un **MVP**.  

“Los más osados dicen que en un fin de semana está lista una aplicación de estas características.”

---

## ✅ 1) Antes de partir: decisiones obligatorias

### 1.1 Elegir el problema (1 por equipo)

Los problemas se entregan como cliente real: **pueden estar incompletos o desordenados**. Cada equipo debe escoger **un (1) problema**:

- **Tema 1**.
- **Tema 2**.
- **Tema 3**.

⚠️ Máximo **3 grupos por tema**.

### 1.2 Elegir herramienta de testing (1 por equipo)

Debes apoyarte en **una** herramienta de testing automatizado (ver **Anexo A**).

⚠️ Máximo **2 grupos por herramienta de testing**.

La elección debe considerar compatibilidad con las tecnologías a utilizar en el proyecto.

Debes elegir bien, porque la herramienta puede impactar tu aplicación, incluso puede existir incompatibilidades que hacen imposible la compatibilidad (algunas son específicas para ciertas tecnologías y lenguajes). Esto impacta el tiempo de desarrollo de esta presentación.

Otra herramienta de pruebas es posible, pero debes inscribirlo en "Aula".

### 1.3 Inscripción en el foro del proyecto (Aula)

En el foro proyecto (Aula) debes inscribir:

- Tema elegido
- Herramienta de testing elegida

⚠️ **Se privilegiará el orden de inscripcción**.

---

## 🧩 2) ¿Qué debes desarrollar?


1) Funcionalidades prioritarias de la aplicación
2) Además incluir (CRUD):
- Listar elementos
- Buscar un elemento específico
- Visualizar el detalle de un elemento
- Agregar un nuevo elemento
- Editar un elemento existente
- Eliminar un elemento

### Ejemplo: VitaCocina

- Listar recetas y consejos
- Buscar recetas (criterios definidos por el equipo)
- Visualizar receta en detalle (con imagen)
- Agregar receta y consejo
- Editar receta y consejo
- Eliminar receta

Si alguno de los casos de uso no aplica a su proyecto, se debe **reemplazar por uno más adecuado**.

---

## 🧪 3) Metodología y forma de trabajo

### 3.1 Reglas de equipo

- Equipos de 3 personas
- Asignar roles internos (incluyendo un líder de equipo).
- Crear organización y repositorio en GitHub.

⚠️ Equipos asignados en aula Moodle.

### 3.2 Flujo de desarrollo y gestión

- Usar GitFlow para el flujo de trabajo.
- Aplicar Kanban con proyecto de tipo "Desarrollo de software" en JIRA.
- Genera cuidadosamente cada hisoria de usuario en el tablero e incluye los criterios de aceptación.
- Crear ítems en el tablero, priorizarlos y estimarlos (horas o story points).
- Tablero **"siempre"** debe estar actualizado.

Herramientas recomendadas: **GitHub + Slack + JIRA**.

### 3.3 Integraciones (configuración)

- Configurar proyecto en JIRA.
- Integrar GitHub + Slack + JIRA (pueden usar configuraciones previas).

⚠️ Si lo prefieres puedes usar Discord en lugar de Slack

---

## ☁️ 4) Plataforma en la nube (sugerida)

Se sugiere usar: **GCP, Azure o AWS**.

🔍 Una VM básica consume aprox. **30-40 USD al mes** si está 100% activa.

ℹ️ Recomendación: Configurar **GitHub Copilot** (gratis para estudiantes).

⚠️ Apagar los servicios en la nube cuando no se estén utilizando.

⚠️ Ver **Anexo B**

---

## 📦 5) Entregables

Se deben cosiderar los siguientes entregables:

1) Repositorio con código fuente en GitHub
2) Documentación del proyecto
3) Cápsula de video explicativa
4) Presentación en clases (si equipo es seleccionado)

### 5.1 Repositorio con código fuente

- **README** de instalación (completo, de acuerdo a definiciones presentadas en aula)
  - Dejar visible enlaces a:
    - Cápsula de video explicativa: Video entrega 1 (link a video/ej: Youtube)
    - Ingregrantes equipo
    - Enlace a Wiki
- **Release notes** (por cada entrega/release)
- **Documentación** de aplicación
- **Licencia**
- **.gitignore**, correctamente configurado
- **Estructura** de carpeta y archivos, de acuerdo a diseño de software
- **Código** de aplicación
- **Información de Contacto y Contribución**

### 5.1.1 **Tag** + Release (obligatorio por entrega)
  - Crear un tag en GitHub que marque exactamente el estado entregado.
  - Publicar un Release asociado al tag (con breve release notes).
  - Convención de nombre del tag: v1.0-entrega1
      - (Entrega 2: v2.0-entrega2, Entrega 3: v3.0-entrega3)
  - El tag debe apuntar a un commit en la rama main (código estable).


### 5.2 Documentación (en Wiki del repositorio)

Debe incluir:

- **Resumen del Proyecto:** objetivos, alcance y propósito.
- **Descripción del Trabajo Realizado:** actividades realizadas, funcionalidades implementadas y logros.
- **Tecnologías de aplicación y su relación con las pruebas:** listado de tecnologías/herramientas y cómo aportan al proceso de pruebas.
- **Evidencia del Trabajo Realizado:** capturas, fragmentos de código, resultados de pruebas u otro material.
- **Estrategia de Pruebas:** metodología adoptada; tipos de pruebas (unitarias, integración, etc.), pruebas de Frontend, Backend, herramientas y cobertura.
- **Supuestos y dependencias:**
  - Listado de condiciones asumidas durante el Desarrollo.
  - Identificación de factores externos que pueden influir en el proyecto (dependencias de terceros, limitaciones tecnológicas, etc.).

Recomendación de estructura:

- **README.md:** visión general + instalación + uso básico + links a doc más detallada + integrantes del equipo + links a videos.
- **Wiki del proyecto:** documentación en profundidad (estrategia de pruebas, supuestos, dependencias, detalles técnicos).
- **Carpeta de documentación:** directorio `docs` para documentos, imágenes, diagramas y material relevante.

 ⚠️ Ver **Anexo B**

### 5.3 El video (qué debe incluir)

- Alcances de la herramienta
- Descripción del trabajo realizado
- Proyecto y dependencias
- Estrategia de pruebas utilizadas
- Procedimiento de ejecución de pruebas
- Resultados y problemas encontrados

### 5.4 Presentación en clase (si eres seleccionado)

- Se realiza el día de entrega.
- Orden de presentación al azar.
- Máximo 25 minutos por equipo.
- Todo el equipo obtiene la misma nota.

---

## 📌 6) Otros

- Declarar supuestos por escrito.
- El diseño gráfico queda a criterio del equipo.
- Preguntas en "foro proyecto en Moodle".
- Configurar organización del proyecto

### 6.1 Fechas relevantes

- Fechas en aula Moodle.

---

# 📎 ANEXOS

## Anexo A — Herramientas de Testing Automatizado (seleccionar una)

- Máximo 2 grupos por herramienta de testing.
  
1. **[Jest](https://jestjs.io/)** is a delightful JavaScript Testing Framework with a focus on simplicity. It works with projects using: Babel, TypeScript, Node, React, Angular, Vue and more! 
1. **[Mocha (Chai)](https://mochajs.org/)** is a feature-rich JavaScript test framework running on Node.js and in the browser, making asynchronous testing simple and fun. Mocha tests run serially, allowing for flexible and accurate reporting, while mapping uncaught exceptions to the correct test cases.
1. **[Jasmine](https://jasmine.github.io/)** is a behavior-driven development framework for testing JavaScript code. It does not depend on any other JavaScript frameworks. It does not require a DOM. And it has a clean, obvious syntax so that you can easily write tests.
1. **[Enzyme](https://enzymejs.github.io/enzyme/)** is a JavaScript Testing utility for React that makes it easier to test your React Components' output. You can also manipulate, traverse, and in some ways simulate runtime given the output. Enzyme's API is meant to be intuitive and flexible by mimicking jQuery's API for DOM manipulation and traversal
1. **[Cypress](https://www.cypress.io/)** is a JavaScript testing automation solution used for web automation. It enables teams to create web test automation scripts. This solution aims to enable frontend developers and test automation engineers to write web tests in the de-facto web language that is JavaScript for web test automation.
1. **[React Testing Library](https://testing-library.com/docs/react-testing-library/intro/)** Testing moderno para React, basado en accesibilidad.
1. **[Vue Test Utils](https://test-utils.vuejs.org/)** Librería oficial para Vue.js.
1. **[Angular Testing Utilities (Karma + Jasmine)](https://angular.dev/guide/testing/utility-apis)** Stack oficial de testing Angular.
1- **[TestCafe](https://testing-library.com/docs/testcafe-testing-library/intro/)**  También usado en UI, pero puede funcionar en flujo unitario para JS apps.
1. **[RSpec (Ruby, estilo BDD)](https://rspec.info/)** Behaviour Driven Development for Ruby. Making TDD Productive and Fun.

En algunos casos se podrá complementar con:
1. **Unittest** Framework estándar de la librería estándar de Python.
1. **PyTest** Más simple y potente que unittest, muy usado en proyectos modernos.

También te puede interesar conocer en este punto soluciones End2End o basadas en Web browser, son similares a Selenium que veremos en la entrega 3:

1. **[Playwraight](https://playwright.dev/)** enables reliable end-to-end testing for modern web apps.
1. **[Puppeteer](https://pptr.dev/)** is a Node.js library which provides a high-level API to control Chrome/Chromium over the DevTools Protocol. Puppeteer runs in headless mode by default, but can be configured to run in full ("headful") Chrome/Chromium.
1. **[Robot Framework](https://robotframework.org/)** is a generic open source automation framework. It can be used for test automation and robotic process automation (RPA). Robot Framework is supported by Robot Framework Foundation. Many industry-leading companies use the tool in their software development.
1. **[Watir](http://watir.com/)** is an open source Ruby library for automating tests. Watir interacts with a browser the same way people do: clicking links, filling out forms and validating text.

Acá algunas alternativas de pago:

1. **Katalon** is a modern, comprehensivenquality management platform Deliver world-class digital experiences with an AI-augmented platform that lets you plan, author and execute automated tests.
1. **TestComplete** is a automated UI testing that covers you from device cloud to packaged apps. Ensure the quality of your application without sacrificing speed or agility with an easy-to-use, GUI test automation tool. Our AI-powered object recognition engine and script or scriptless flexibility is unmatched, letting you test every desktop, web, and mobile application with ease. (Solo 15 días de prueba)

> La elección debe considerar compatibilidad con las tecnologías del equipo.

**Debes elegir bien, porque la elección que hagas debe permitir cumplir con el objetivo de solicitado para la aplicación y además la elección puede tener impacto en tu aplicación, es decir algunas de las herramientas listadas son específicas para ciertas tecnologías, por lo tanto si quieres usarla deberás usar determinados lenguajes de programación. Todo lo anterior tiene un impacto en el tiempo de desarrollo de esta presentación.**

**Otra herramienta de pruebas es posible, pero debes inscribirlo en aula**

---

## Anexo B — Créditos y links de Nube

Se sugiere usar: GCP, Azure o AWS

### Créditos Nube:

- **Azure**
  - [100USD en crédito de Azure, sin tarjeta de crédito](https://aws-experience.com/latam/smb/exclusive-offers/aws-credits) 

- **AWS**
  - [AWS Educate](https://aws.amazon.com/es/education/awseducate/)
  - [$300 en créditos de AWS](https://aws-experience.com/latam/smb/exclusive-offers/aws-credits)
  - [$200 free Tier](https://aws.amazon.com/es/free)

- **GCP**
  - [Google Cloud para alumnos](https://cloud.google.com/edu/students)
  - [Obtén y canjea créditos educativos](https://cloud.google.com/billing/docs/how-to/edu-grants)
 
- **IA con Gemini**
  - [L#300 La era Gemini para desarrolladores y empresas](https://cloud.google.com/ai/gemini)

> 🔍 Una VM básica consume aprox. 30-40 USD al mes si está 100% activa.

> ℹ️ Recomendación: Configurar GitHub Copilot (gratis para estudiantes).

> ⚠️ Apagar los servicios en la nube cuando no se estén utilizando.

---

## Anexo C — Wiki en GitHub (Home + Pages)

En GitHub tenemos:

- **Home** = la página principal (la portada).
- **Pages** = el listado de páginas de la Wiki (menú lateral / lista de páginas).

La idea es que **Home** sea solo navegación + orientación, y que **Pages** tenga páginas separadas: unas “del proyecto” y otras “de entregas”.

### Cómo debería verse el Home (portada)

**Home (contenido recomendado):**

- Qué es este repo: nombre del proyecto + propósito.
- Cómo partir (links directos):
  - Instalación / ejecución local (si lo documentan en Wiki; si no, link al README)
  - Cómo ejecutar pruebas
- Entregas (links):
  - Entrega 1 (link)
  - Entrega 2 (placeholder)
  - Entrega 3 (placeholder)
- Documentación base del proyecto (links):
  - Resumen del Proyecto
  - Arquitectura y Diseño
  - Tecnologías y Stack
  - Estrategia de Pruebas (Global)
  - Supuestos y Dependencias (Global)
- Evidencias y recursos (links):
  - Evidencias / Bitácora
  - Release/Tag Entrega 1: link al release/tag v1.0-entrega1

En simple: **Home es un índice**, no un lugar para explicar todo.

### Cómo debería verse la lista Pages (estructura real en GitHub Wiki)

En Pages, yo lo ordenaría con nombres que se agrupen solos alfabéticamente (GitHub Wiki no permite carpetas reales, pero el prefijo ayuda).

**Grupo 1 — Páginas del proyecto (genéricas)**

Estas no son “por entrega”, sino cosas que valen para todo el semestre.

- Proyecto - Resumen  
  - Objetivo, alcance, usuarios, qué problema resuelve
- Proyecto - Tecnologías y Stack  
  - Tecnologías elegidas + breve justificación + cómo se relaciona con pruebas
- Proyecto - Arquitectura y Diseño  
  - Diagrama simple + estructura del repo + decisiones relevantes
- Proyecto - Estrategia de Pruebas  
  - Plan global: qué tipos de pruebas existen en el proyecto y cómo irá evolucionando en E1/E2/E3
- Proyecto - Supuestos y Dependencias  
  - Supuestos generales + dependencias externas/limitaciones
- Proyecto - Evidencias  
  - Capturas, links a PRs, resultados importantes, etc.

**Grupo 2 — Páginas por entrega (específicas)**

Estas sí se evalúan por hito. La clave es que la página **Entrega 1** tenga H1 = “Entrega 1”.

- Entrega 1  
  - (página evaluable, con el detalle de lo hecho en E1)
- Entrega 2 (placeholder)
- Entrega 3 (placeholder)

### Plantilla mínima recomendada para la página “Entrega 1”

(para que corrijas rápido y sea consistente)

- Entrega 1
  - Objetivo de la entrega
  - Alcance implementado (CRUD)
  - Cómo ejecutar el sistema (local)
  - Pruebas: qué se probó + cómo ejecutar + resultados
  - Evidencia (capturas de pantalla JIRA/Slack - links PR -release - tag)
  - Problemas encontrados / pendientes
  - Supuestos y dependencias específicas de E1 (si aplica)

---
## Anexo D — Configurar organización del proyecto (Identidad)

- Nombre y “handle” claros (ej: inf331-equipo-7 o hands-on-<tema>-<equipo>).
- Logo/Avatar consistente (simple, legible).
- Description (puede apuntar al repo principal o a la Wiki).
- README público de la org (.github/profile/README.md) con:
  - propósito del proyecto
  - links: repo, Wiki, etc.

---
