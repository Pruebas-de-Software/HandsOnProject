# Instrucciones entregas proyecto Semestre 1 2026

## Objetivo global del proyecto

“En 3 entregas construiremos una app web con calidad creciente: funcionalidad → CI/CD → E2E, dejando evidencia y trazabilidad.”

### “Definition of Done” resumida por entrega

- Entrega1: Requisitos principales + CRUD + tests corriendo + documentación base + tag/release
- Entrega2: Pipeline automático por cambios + integraciones (GitHub/Slack) + nuevos reqs + evidencia
- Entrega3: Tests E2E + corren en pipeline headless + falla si falla + artefactos + notificaciones
---

### 🔹 Entrega 1: Construcción inicial aplicación y pruebas automatizadas

- Primera entrega de aplicación.
- Desarrollo de un CRUD funcional, y funcionalidades prioritarias de aplicación web definida por el equipo.
- Implementación de pruebas automatizadas iniciales según herramienta escogida

📄 [Ver detalles de la Entrega 1](./entrega1.md)


### 🔹 Entrega 2: CI/CD con Jenkins

- Segunda entrega de aplicación
- Instalación y configuración de Jenkins.
- Creación de un pipeline de integración y despliegue continuo.
- Entrega de nuevos requerimientos y automatización de su despliegue.

📄 [Ver detalles de la Entrega 2](./entrega2.md)


### 🔹 Entrega 3: Pruebas de interfaz con Selenium

- Tercera entrega de aplicación
- Desarrollo de pruebas de interfaz usando Selenium o Playwright.
- Integración de pruebas al pipeline CI/CD.
- Ejecución continua y notificaciones automáticas de resultados.

📄 [Ver detalles de la Entrega 3](./entrega3.md)

---

### ¿Qué se entrega siempre? (común a las 3 entregas)

- Repo GitHub
- Documentación actualizada
- Video + (release/tag por entrega)

### Criterios de evaluación
- Calidad del código
- Funcionalidad
- Pruebas/calidad
- Automatización (CI/CD/E2E según entrega)
- Documentación/evidencia
- Gestión (Jira + GitFlow + PRs)

## Reglas operativas para evitar el caos
- Convención de tags: v1.0-entrega1, v2.0-entrega2, v3.0-entrega3
- PR obligatorio a main (y “main protegido” desde E1)
- **Una rama = un objetivo** (no mezclar feature + tests + docs en la misma).
- **Nombre corto y claro**, sin tildes, sin espacios.
- Siempre incluir **ID de Jira** (o Issue) para trazabilidad.
- Merge a `develop` vía **Pull Request** (y a `main` solo con release/tag).

### Convención de nombres de ramas (Branch Naming)

Objetivo: mantener el repositorio ordenado, trazable (Jira/GitHub) y evitar caos.

#### 1) Ramas principales (fijas)

- `main` → estable / entregable
- `develop` → integración de trabajo (si usan GitFlow)

#### 2) Ramas de trabajo (por tipo)

**Formato general:**
```
<tipo>/<id-jira>-<descripcion-corta-kebab-case>
```

##### Tipos sugeridos
- `feature/` → nueva funcionalidad
- `fix/` → bug
- `test/` → creación/mejora de pruebas
- `ci/` → CI/CD, Jenkins, pipelines
- `docs/` → documentación (README/Wiki)
- `refactor/` → refactor sin cambio funcional
- `chore/` → tareas menores (deps, config, limpieza)


#### 3) Ejemplos

- `feature/LIC-12-crear-licitacion`
- `fix/LIC-18-error-validacion-fecha`
- `test/LIC-25-pruebas-unitarias-repositorio`
- `ci/LIC-31-jenkinsfile-pipeline`
- `docs/LIC-40-actualizar-wiki-entrega2`
- `refactor/LIC-44-separar-servicios`
- `chore/LIC-50-actualizar-dependencias`

---
