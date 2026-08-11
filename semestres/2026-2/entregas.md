# HandsOnProject INF331

**Semestre 2 · 2026**  
**Asignatura:** INF331 — Pruebas de Software  
**Universidad Técnica Federico Santa María**

---

## 1. Propósito del proyecto

HandsOnProject es una experiencia práctica y progresiva en la que cada equipo construirá una aplicación web de código abierto y aplicará prácticas de calidad similares a las utilizadas en proyectos reales de software.

El proyecto no consiste únicamente en desarrollar funcionalidades. Su propósito es aprender a construir software **verificable, trazable, automatizado y reproducible**, incorporando las pruebas desde el inicio y elevando gradualmente el nivel de calidad en tres entregas:

> **Entrega 1: producto y pruebas automatizadas → Entrega 2: integración y despliegue continuos → Entrega 3: pruebas E2E integradas al pipeline.**

Al finalizar el semestre, el equipo deberá contar con una aplicación funcional desplegada, un repositorio profesional, una estrategia de pruebas en distintos niveles, un pipeline CI/CD y evidencias que permitan verificar la calidad del producto.

---

## 2. Temas disponibles

Cada equipo deberá escoger uno de los siguientes proyectos:

1. [RentSmart: Arriendo de espacios entre particulares](./tema1.md)
2. [Mira: Gestión de proyectos Scrum y Kanban](./tema2.md)
3. [CrowdStarter: Plataforma web de crowdfunding](./tema3.md)

Las descripciones representan una **especificación inicial deliberadamente incompleta**. Cada equipo deberá analizar el problema, declarar supuestos, resolver dudas con el equipo docente y transformar la idea en requisitos verificables.

### 2.1 Flujo de negocio central de cada tema

| Tema | Flujo principal que debe orientar el MVP |
| --- | --- |
| **RentSmart** | Un propietario publica un espacio; otro usuario lo busca, revisa su disponibilidad y solicita o realiza una reserva. |
| **Mira** | Un usuario crea o integra una organización/proyecto, incorpora trabajo al backlog y gestiona su avance mediante un tablero Kanban o un Sprint. |
| **CrowdStarter** | Un creador publica una campaña; otro usuario la descubre, revisa su información y realiza un aporte mediante el flujo de pago definido. |

El CRUD es una base técnica necesaria, pero **no reemplaza el flujo de negocio**. Una aplicación que solo permita crear, editar y eliminar registros, sin resolver el proceso central del tema, no constituye un MVP suficiente.

---

## 3. Progresión de las entregas

### 🔹 Entrega 1: Producti inicial aplicación y pruebas automatizadas

- Primera entrega de aplicación.
- MVP funcional, persistencia y flujo principal
- Pruebas automatizadas iniciales, trazabilidad y documentación base

📄 [Ver detalles de la Entrega 1](./entrega1.md)


### 🔹 Entrega 2: CI/CD

- Segunda entrega de aplicación
- Instalación y configuración de herramienta CI/CD.
- Nuevos requisitos y correcciones comprometidas
- Creación de un pipeline de integración y despliegue continuo.

📄 [Ver detalles de la Entrega 2](./entrega2.md)


### 🔹 Entrega 3: Calidad de extremo a extremo

- Tercera entrega de aplicación
- Requisitos finales
- Pruebas E2E/UI en modo headless, artefactos, fallos visibles y
- Notificaciones automáticas de resultados.

📄 [Ver detalles de la Entrega 3](./entrega3.md)

Cada entrega es incremental. Los requisitos de una entrega anterior **continúan vigentes** en las siguientes, salvo que se indique expresamente lo contrario.

---

## 4. Reglas comunes para todo el semestre

### 4.1 Equipos y responsabilidades

- Los equipos estarán formados por tres o cuatro integrantes, según la asignación publicada en Aula.
- Cada equipo deberá definir responsabilidades internas. Estas pueden rotar durante el semestre.
- Todo integrante debe participar en el desarrollo, las pruebas, la revisión o la documentación técnica.
- La contribución se verificará mediante Jira, commits, ramas, Pull Requests, revisiones y evidencias de colaboración.
- El trabajo en pares o *mob programming* es válido y recomendable.

La cantidad de commits no determina por sí sola la contribución individual. Se evaluará el valor, la consistencia y la trazabilidad del trabajo realizado.

### 4.2 Gestión del trabajo

El proyecto se administrará mediante un tablero Kanban en Jira, o una herramienta equivalente autorizada por el equipo docente.

El tablero deberá:

- Contener historias de usuario, tareas, pruebas, defectos y actividades técnicas;
- Incluir criterios de aceptación verificables en las historias de usuario;
- Mostrar prioridad, responsable y estimación en horas o *story points*;
- Mantenerse actualizado durante todo el desarrollo;
- Reflejar el trabajo real del equipo, no reconstruirse únicamente al final de la entrega.

Cada historia debería expresar, como mínimo:

```text
Como <tipo de usuario>
Quiero <capacidad>
Para <beneficio o propósito>.
```

Sus criterios de aceptación deben describir comportamientos observables. Se recomienda utilizar el formato **Dado / Cuando / Entonces** cuando facilite su comprensión.

### 4.3 Trazabilidad mínima

Debe ser posible recorrer la siguiente cadena:

> **Requisito o historia → ítem de Jira → rama → commits → Pull Request → pruebas → resultado en pipeline → release.**

Para ello:

- Cada rama y Pull Request debe incluir el identificador del ítem relacionado;
- Cada requisito implementado debe asociarse con sus pruebas;
- Los defectos relevantes deben registrarse con pasos de reproducción, resultado esperado, resultado obtenido, severidad y evidencia;
- La Wiki debe enlazar las evidencias más importantes, evitando capturas aisladas sin contexto.

### 4.4 Flujo Git y Pull Requests

Ramas permanentes:

- `main`: Versión estable y entregable;
- `develop`: Integración del trabajo del equipo.

Ramas de trabajo:

```text
<tipo>/<id-jira>-<descripcion-corta-en-kebab-case>
```

Tipos recomendados:

- `feature/`: Nueva funcionalidad;
- `fix/`: Corrección de un defecto;
- `test/`: Creación o mejora de pruebas;
- `ci/`: Pipeline, despliegue o automatización;
- `docs/`: Documentación;
- `refactor/`: Refactorización sin cambio funcional;
- `chore/`: Configuración, dependencias o mantenimiento.

Ejemplos:

```text
feature/MIR-12-crear-proyecto
fix/MIR-18-validar-fecha-sprint
test/MIR-25-pruebas-servicio-tareas
ci/MIR-31-pipeline-jenkins
docs/MIR-40-wiki-entrega-2
```

Reglas obligatorias:

- Una rama debe perseguir un objetivo coherente y acotado;
- Los cambios ingresan a `develop` mediante Pull Request;
- La versión entregable ingresa a `main` mediante Pull Request de release;
- No se realizan *pushes* directos a `main`;
- `main` debe estar protegida desde la Entrega 1;
- Cada Pull Request debe explicar qué cambia, cómo se probó y qué ítem resuelve;
- Antes de fusionar se debe realizar, como mínimo, una revisión de otro integrante;
- No se deben incluir credenciales, secretos, archivos `.env` reales ni datos personales en el repositorio.

### 4.5 Versiones, tags y releases

Cada entrega deberá cerrarse desde un commit estable en `main`:

| Entrega | Tag obligatorio |
| --- | --- |
| Entrega 1 | `v1.0-entrega1` |
| Entrega 2 | `v2.0-entrega2` |
| Entrega 3 | `v3.0-entrega3` |

Cada tag deberá tener un **GitHub Release** asociado que indique:

- Funcionalidades incorporadas;
- Defectos corregidos;
- Pruebas ejecutadas y su resultado;
- Limitaciones o problemas conocidos;
- Instrucciones especiales de instalación o actualización, si corresponden.

### 4.6 Repositorio mínimo

Desde la Entrega 1, el repositorio deberá contener:

- Código fuente de la aplicación y las pruebas;
- `README.md` con propósito, integrantes, instalación, configuración, ejecución, pruebas y enlaces principales;
- `.gitignore` correcto;
- Archivo `.env.example` sin secretos, cuando corresponda;
- Licencia de código abierto;
- Estructura de carpetas coherente;
- Scripts o comandos reproducibles para instalar, levantar, probar y construir la aplicación;
- Directorio `docs/` para diagramas, imágenes o documentación versionada que no pertenezca a la Wiki;
- Información para contribuir al proyecto.

### 4.7 Documentación en la Wiki

La página **Home** debe funcionar como índice y enlazar las páginas del proyecto y de cada entrega.

Páginas base recomendadas:

- `Proyecto - Resumen y alcance`
- `Proyecto - Requisitos y trazabilidad`
- `Proyecto - Arquitectura y tecnologías`
- `Proyecto - Estrategia de pruebas`
- `Proyecto - Supuestos y dependencias`
- `Proyecto - Evidencias`
- `Entrega 1`
- `Entrega 2`
- `Entrega 3`

La documentación debe actualizarse durante el trabajo. Una captura de pantalla demuestra un estado puntual, pero no reemplaza una explicación técnica, un enlace verificable ni un resultado reproducible.

### 4.8 Uso de herramientas de inteligencia artificial

Se permite utilizar asistentes de inteligencia artificial como apoyo. El equipo deberá documentar brevemente:

- Herramientas utilizadas y propósito;
- Elementos relevantes generados o modificados con apoyo de IA;
- Forma en que se revisó y validó su resultado.

El equipo sigue siendo responsable de comprender, probar y explicar todo el código entregado.

### 4.9 Evidencia común

Toda afirmación importante debe ser verificable. Se privilegiarán enlaces y artefactos reproducibles por sobre capturas de pantalla.

Ejemplos de evidencia válida:

- Pull Request revisado;
- Historia de usuario con criterios de aceptación;
- Ejecución de pruebas con reporte;
- Enlace a un pipeline exitoso y a uno fallido de manera controlada;
- Reporte de cobertura, cuando la herramienta lo permita;
- Despliegue accesible;
- Release y tag;
- Registro de defecto y su corrección.

### 4.10 Entregables comunes

En cada hito se deberá entregar:

1. Enlace al repositorio de GitHub;
2. Versión estable en `main`, tag y release correspondiente;
3. Wiki actualizada;
4. Cápsula de video explicativa;
5. Presentación en clases, solo entregas 1 y 3

Las fechas, el medio de entrega y la selección de equipos que presentan se publicarán en Aula.

---
