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
1. **Puppeteer**: es una biblioteca de Node.js que proporciona una API de alto nivel para controlar Chrome/Chromium mediante el Protocolo DevTools. Puppeteer se ejecuta en modo sin cabeza por defecto, pero puede configurarse para ejecutarse en modo completo ("headful") Chrome/Chromium.&#8203;:contentReference[oaicite:0]{index=0}

2. **Jest**: :contentReference[oaicite:1]{index=1}&#8203;:contentReference[oaicite:2]{index=2}

3. **Mocha (Chai)**: :contentReference[oaicite:3]{index=3}&#8203;:contentReference[oaicite:4]{index=4}

4. **Jasmine**: :contentReference[oaicite:5]{index=5}&#8203;:contentReference[oaicite:6]{index=6}

5. **Enzyme**: es una utilidad de pruebas de JavaScript para React que facilita la prueba de la salida de tus Componentes React. También puedes manipular, recorrer y, de alguna manera, simular el tiempo de ejecución dada la salida. La API de Enzyme está diseñada para ser intuitiva y flexible, imitando la API de jQuery para manipulación y recorrido del DOM.&#8203;:contentReference[oaicite:7]{index=7}

6. **Cypress**: es una solución de automatización de pruebas de JavaScript utilizada para la automatización web. Permite a los equipos crear scripts de automatización de pruebas web. Esta solución tiene como objetivo permitir a los desarrolladores frontend e ingenieros de automatización de pruebas escribir pruebas web en el lenguaje web por defecto que es JavaScript para la automatización de pruebas web.&#8203;:contentReference[oaicite:8]{index=8}

7. **Robot Framework**: es un framework de automatización genérico de código abierto. Puede ser utilizado para la automatización de pruebas y la automatización de procesos robóticos (RPA). Robot Framework es apoyado por Robot Framework Foundation. Muchas empresas líderes en la industria utilizan la herramienta en su desarrollo de software.&#8203;:contentReference[oaicite:9]{index=9}

8. **Katalon**: es una plataforma moderna y completa de gestión de calidad que ofrece experiencias digitales de clase mundial con una plataforma aumentada por IA que te permite planificar, crear y ejecutar pruebas automatizadas.&#8203;:contentReference[oaicite:10]{index=10}

9. **TestComplete**: es una herramienta de pruebas de UI automatizadas que cubre desde la nube de dispositivos hasta aplicaciones empaquetadas. Asegura la calidad de tu aplicación sin sacrificar velocidad o agilidad con una herramienta de automatización de pruebas GUI fácil de usar. Nuestro motor de reconocimiento de objetos impulsado por IA y la flexibilidad de script o sin script es inigualable, permitiéndote probar cada aplicación de escritorio, web y móvil con facilidad. (Solo 15 días de prueba)&#8203;:contentReference[oaicite:11]{index=11}

10. **Watir**: es una biblioteca Ruby de código abierto para automatizar pruebas. Watir interactúa con un navegador de la misma manera que lo hacen las personas: haciendo clic en enlaces, completando formularios y validando texto.&#8203;:contentReference[oaicite:12]{index=12}

11. **Testsigma**: es una herramienta de pruebas automatizadas de UI web intuitiva, rica en características y asequible. Testsigma utiliza IA para crear pruebas automatizadas estables y confiables más rápido que nunca y para acelerar las ejecuciones y el mantenimiento de tus pruebas automatizadas. No se requieren habilidades de codificación.&#8203;:contentReference[oaicite:13]{index=13}

12. **unittest**: El framework de pruebas unitarias fue inspirado originalmente por JUnit y tiene un sabor similar a los principales frameworks de pruebas unitarias en otros lenguajes. Soporta la automatización de pruebas, el intercambio de código de configuración y desmontaje para pruebas, la agregación de pruebas en colecciones y la independencia de las pruebas del framework de informes.&#8203;:contentReference[oaicite:14]{index=14}



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

- Inscribir en el foro (Preoyecto en Moodle):
  - Tema elegido
  - Herramienta de testing elegida

> ⚠️ Máximo 2 grupos por herramienta de testing.

- Si un equipo quiere utilizar alguna herramienta distinta puede hacerlo, pero debe informar y cumplir con el objetivo de probar la aplicación.
- Declarar supuestos por escrito.
- El diseño gráfico queda a criterio del equipo.
- Preguntas en "foro proyecto en Moodle"

### 3.3 Fechas Relevantes

- Fechas en aula Moodle

### 3.4 Entregables

- Repositorio con código fuente en GitHub
- README de instalación (completo)
- **Cápsula de video explicativa** alojada en el repositorio

#### El video debe incluir:

- Alcances de la herramienta
- Descripción del trabajo realizado
- Proyecto y dependencias
- Estrategia de pruebas utilizadas
- Procedimiento de ejecución de pruebas
- Resultados y problemas encontrados

#### Documentación (en Markdown en el mismo repo):

- Mismos puntos del video
- Infraestructura de la aplicación y su relación con las pruebas

### 3.5 Presentación en Clase

- Se realiza el día de entrega.
- Orden de presentación al azar.
- **Máximo 25 minutos por equipo**.
- Todo el equipo obtiene la misma nota.

---

## 👥 4. Equipos

*Se asignan y publican según inscripciones. Cada equipo elige su tema y herramienta en los canales oficiales.*

---

> ✅ Para preguntas o aclaraciones, usar el foro de la sección correspondiente.

