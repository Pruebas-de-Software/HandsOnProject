# 📚 Material de Apoyo SW + CI/CD

---

## 💻 Material desarrollo de SW

🔧 Metodologías para desarrollo de Software, frameworks y creación de productos:

- [Waterfall (la verdadera historia)](https://aula.usm.cl/draftfile.php/541939/user/draft/166352627/waterfall.pdf)  
- [Open UP ¿Qué es?](https://licklider.cl/epf/)  
- [Shape UP](https://basecamp.com/shapeup)  
- [Scrum y XP desde la trinchera](https://leanagiletraining.com/wp-content/uploads/2020/03/Scrum-and-XP-from-the-Trenches-2nd-edition.pdf)  
- [Kanban (intro)](https://aula.usm.cl/draftfile.php/541939/user/draft/166352627/Introducci%C3%B3n_Kanban%20v2.2.pdf)  
- [Scrumban](https://www.atlassian.com/agile/project-management/scrumban#:~:text=Agile%20project%20management.-,What%20is%20Scrumban%3F,work%2Din%2Dprogress%20limitations.)  

---

## 🌱 Material Git y relacionados

### 🐙 Git

- [El libro completo Pro Git (Scott Chacon y Ben Straub)](https://git-scm.com/book/en/v2)  
- [Hoja de referencia Git](https://training.github.com/downloads/es_ES/github-git-cheat-sheet/)  
- [Simulador Git](https://learngitbranching.js.org/?locale=es_ES)  

🔧 **Herramientas:**
- [GitKraken](https://www.gitkraken.com/)  
- [Git4Windows](https://gitforwindows.org/)  

### 🐱 GitHub

- 📖 **GitHub Docs**: Documentación oficial de GitHub sobre repositorios, ramas y colaboración.  
  👉 [https://docs.github.com/es](https://docs.github.com/es)  
  - 📂 [Documentación de Repositorios](https://docs.github.com/es/repositories)  

### 🌳 Flujos de Trabajo con Git

- **🔀 GitFlow**
  - [A successful Git branching model](https://nvie.com/posts/a-successful-git-branching-model/)  
  - [GitFlow workflow (Atlassian)](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow#:~:text=What%20is%20Gitflow%3F,lived%20branches%20and%20larger%20commits.)  

- **🌲 Trunk**
  - [Trunk Based Development (Google)](https://cloud.google.com/architecture/devops/devops-tech-trunk-based-development?hl=es-419)  
  - [Trunk Based Development (Atlassian)](https://www.atlassian.com/continuous-delivery/continuous-integration/trunk-based-development)  

- **🚢 Ship / Show / Ask**
  - [Ship / Show / Ask (Martin Fowler)](https://martinfowler.com/articles/ship-show-ask.html)  
  - [Estrategia de Git: Ship / Show / Ask](https://midu.dev/ship-show-ask-estrategia-git/)  

---

## ⚙️ DevOps

### 🤝 GitHub + Jira + Slack

- **Integraciones GitHub + Slack**  
  - [Slack + GitHub](https://slack.github.com/)  
  - [GitHub App para Slack](https://personal-slacksede.slack.com/apps/A01BP7R4KNY-github?tab=more_info)  

### 📘 Guía DevOps

- [Requisitos para examen (incluye enlaces)](https://devopsinstitute.com/wp-content/uploads/2021/03/DOFD-v3.3-Spanish-Exam-Study-Guide_01Mar2021.pdf)  
- [Study Guide (English version)](https://www.devopsinstitute.com/wp-content/uploads/2021/03/DOFD-v3.3-English-Exam-Study-Guide_01Mar2021.pdf)  

### 📚 Libros DevOps

- [Bibliografía del curso](https://aula.usm.cl/mod/page/view.php?id=5688251)  

---

## ☁️ Créditos Nube

- **🔵 Azure**  
  - [100 USD en crédito de Azure (sin tarjeta de crédito)](https://aws-experience.com/latam/smb/exclusive-offers/aws-credits)  
  - [Créala en pocos pasos](https://aula.usm.cl/mod/page/view.php?id=4162228)  

- **🟠 AWS**  
  - [AWS Educate](https://aws.amazon.com/es/education/awseducate/)  
  - [$300 en créditos de AWS](https://aws-experience.com/latam/smb/exclusive-offers/aws-credits)  
  - [$200 free Tier](https://aws.amazon.com/es/free/)  

- **🟢 GCP**  
  - [Google Cloud para alumnos](https://cloud.google.com/edu/students)  
  - [Canjea créditos educativos](https://cloud.google.com/billing/docs/how-to/edu-grants)  

---
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
# :wave: Fundamentos de GitHub 

## :octocat: Git y GitHub

Git es un **Sistema de Control de Versiones distribuido (VCS)**, lo que significa que es una herramienta útil para rastrear fácilmente los cambios en tu código, colaborar y compartir. Con Git puedes seguir los cambios que haces en tu proyecto, de modo que siempre tengas un registro de en qué trabajaste y puedas volver con facilidad a una versión anterior si lo necesitas. También facilita el trabajo con otras personas: varios grupos pueden colaborar en el mismo proyecto y fusionar sus cambios en una fuente final.

GitHub es una manera de usar todo el poder de Git en línea, con una interfaz fácil de usar. Se utiliza en todo el mundo del software y más allá para colaborar y mantener el historial de los proyectos.

GitHub es el hogar de algunas de las tecnologías más avanzadas del mundo. Ya sea que estés visualizando datos o creando un nuevo juego, en GitHub hay toda una comunidad y un conjunto de herramientas que pueden llevarte al siguiente nivel. Este curso comienza con lo básico de GitHub, pero más adelante profundizaremos en el resto.

## :octocat: Entendiendo el flujo de GitHub 

El flujo de GitHub es un flujo de trabajo liviano que te permite experimentar y colaborar en tus proyectos con facilidad, sin el riesgo de perder tu trabajo anterior.

### Repositorios

Un repositorio es donde ocurre el trabajo de tu proyecto —piénsalo como la carpeta de tu proyecto—. Contiene todos los archivos de tu proyecto y el historial de revisiones. Puedes trabajar dentro de un repositorio por tu cuenta o invitar a otros a colaborar contigo en esos archivos.

### Clonado 

Cuando se crea un repositorio con GitHub, se almacena de forma remota en la ☁️. Puedes **clonar** un repositorio para crear una copia local en tu computadora y luego usar Git para sincronizar ambos. Esto facilita corregir problemas, agregar o eliminar archivos y subir *commits* más grandes. También puedes usar la herramienta de edición que prefieras en lugar de la interfaz de GitHub. Clonar un repositorio también descarga todos los datos del repositorio que GitHub tiene en ese momento, incluidas todas las versiones de cada archivo y carpeta del proyecto. Esto puede ser útil si experimentas con tu proyecto y luego te das cuenta de que te gustaba más una versión anterior.  
Para aprender más sobre cómo clonar, lee ["Cloning a Repository"](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository).

### Hacer *commit* y *push*
**Hacer *commit*** y **hacer *push*** son las formas de agregar los cambios que hiciste en tu máquina local al repositorio remoto en GitHub. De esa forma, tu profesor y/o tu equipo podrán ver tu trabajo más reciente cuando estés listo para compartirlo. Puedes hacer un *commit* cuando hayas realizado cambios en tu proyecto que quieras “marcar como punto de control”. También puedes agregar un **mensaje de *commit*** útil para recordarte a ti o a tu equipo qué trabajo hiciste (por ejemplo: “Se agregó un README con información sobre nuestro proyecto”).

Cuando tengas uno o varios *commits* que estén listos para añadir a tu repositorio, puedes usar el comando *push* para subir esos cambios a tu repositorio remoto. Hacer *commit* y *push* puede sentirse nuevo al principio, pero te prometemos que te acostumbrarás 🙂.

## 💻 Términos de GitHub que debes conocer 

### Repositorios 
Ya hablamos de los repositorios: ahí es donde ocurre el trabajo de tu proyecto, pero hablemos un poco más de sus detalles. A medida que uses más GitHub tendrás muchos repositorios, lo que al principio puede resultar confuso. Afortunadamente, tu ["tablero de GitHub"](https://docs.github.com/en/github/setting-up-and-managing-your-github-user-account/about-your-personal-dashboard) te ayuda a navegar fácilmente a tus repositorios y ver información útil sobre ellos. ¡Asegúrate de haber iniciado sesión para verlo!

Los repositorios también contienen **README**. Puedes añadir un archivo README a tu repositorio para contarle a otras personas por qué tu proyecto es útil, qué pueden hacer con él y cómo pueden usarlo. Estamos usando este README para comunicarte cómo aprender Git y GitHub. 😄  
Para aprender más sobre repositorios, lee ["Creating, Cloning, and Archiving Repositories"](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/about-repositories) y ["About README's"](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/about-readmes).

### Ramas (*Branches*)
Puedes usar ramas en GitHub para aislar trabajo que todavía no quieres fusionar con tu proyecto final. Las ramas te permiten desarrollar funcionalidades, corregir errores o experimentar con ideas nuevas de forma segura en un área contenida de tu repositorio. Normalmente, puedes crear una nueva rama desde la rama predeterminada de tu repositorio —*main*—. Esto crea una nueva copia de trabajo de tu repositorio para que experimentes. Una vez que tus cambios hayan sido revisados por un compañero, o estés satisfecho con ellos, puedes fusionarlos en la rama predeterminada de tu repositorio.  
Para aprender más sobre ramas, lee ["About Branches"](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-branches).

### *Forks*
Un *fork* es otra forma de copiar un repositorio, pero suele utilizarse cuando quieres contribuir al proyecto de otra persona. Hacer *fork* de un repositorio te permite experimentar libremente con cambios sin afectar el proyecto original y es muy popular al contribuir a proyectos de software de código abierto.  
Para aprender más sobre *forks*, lee ["Fork a repo"](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo).

### Pull requests
Cuando trabajas con ramas, puedes usar un *pull request* para contarles a otros sobre los cambios que quieres hacer y pedir su retroalimentación. Una vez abierto un *pull request*, puedes discutir y revisar los cambios potenciales con colaboradores y añadir más cambios si es necesario. Puedes agregar personas específicas como revisores de tu *pull request*, lo que muestra que quieres sus comentarios sobre tus cambios. Cuando un *pull request* está listo, se puede fusionar en tu rama *main*.  
Para aprender más sobre *pull requests*, lee ["About Pull Requests"](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests).

### Issues
Los *issues* son una forma de rastrear mejoras, tareas o errores en tu trabajo en GitHub. Son una gran manera de llevar registro de todas las tareas en las que quieres trabajar para tu proyecto y de informar a otros qué planeas hacer. ¡También puedes usar *issues* para contarle a tu proyecto de código abierto favorito sobre un error que encontraste o una funcionalidad que sería genial agregar!

Para proyectos más grandes, puedes llevar el control de muchos *issues* en un tablero de proyecto. GitHub Projects te ayuda a organizar y priorizar tu trabajo y puedes leer más al respecto [en este documento "About Project boards"](https://docs.github.com/en/github/managing-your-work-on-github/about-project-boards). Probablemente no necesites un tablero de proyecto para tus tareas, pero cuando avances a proyectos más grandes, ¡son una gran forma de organizar el trabajo de tu equipo!  
También puedes vincular *pull requests* e *issues* para mostrar que una solución está en progreso y para cerrar automáticamente el *issue* cuando alguien fusione el *pull request*.  
Para aprender más sobre *issues* y cómo vincularlos a tus *pull requests*, lee ["About Issues"](https://docs.github.com/en/github/managing-your-work-on-github/about-issues).

### Tu perfil de usuario
Tu página de perfil le cuenta a la gente la historia de tu trabajo a través de los repositorios que te interesan, las contribuciones que has hecho y las conversaciones que has tenido. También puedes darle al mundo una vista única de quién eres con el README de tu perfil. ¡Puedes usar tu perfil para que futuros empleadores sepan todo sobre ti!  
Para aprender más sobre tu perfil de usuario y sobre cómo agregar y actualizar tu README de perfil, lee ["Managing Your Profile README"](https://docs.github.com/en/github/setting-up-and-managing-your-github-profile/managing-your-profile-readme).

### Uso de Markdown en GitHub 
Quizás ya lo notaste, pero puedes agregar algo de estilo a tus *issues*, *pull requests* y archivos. ["Markdown"](https://guides.github.com/features/mastering-markdown/) es una forma sencilla de dar formato a tus *issues*, *pull requests* y archivos con una sintaxis simple. Esto puede ayudar a organizar tu información y hacerla más fácil de leer para otros. ¡También puedes insertar GIFs e imágenes para ayudar a transmitir tu punto!  
Para aprender más sobre el uso del Markdown de GitHub, lee ["Basic Writing and Formatting Syntax"](https://docs.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax).

### Interacción con la comunidad de GitHub
La comunidad de GitHub es enorme. Hay muchos tipos de personas que usan GitHub en su día a día: estudiantes como tú, desarrolladores profesionales, aficionados que trabajan en proyectos de código abierto y exploradores que recién se adentran en el mundo del desarrollo de software por su cuenta. Hay muchas maneras de interactuar con la comunidad más amplia de GitHub, pero aquí tienes tres lugares por donde empezar. 

#### Marcar repositorios con estrella (*Starring*) 
Si encuentras un repositorio interesante o quieres seguirle la pista, ¡márcalo con una estrella! Cuando marcas un repositorio con estrella, también se usa como una señal para ofrecerte mejores recomendaciones en github.com/explore. Si quieres volver a tus repositorios con estrella, puedes hacerlo desde tu perfil de usuario.  
Para aprender más sobre marcar repositorios con estrella, lee ["Saving Repositories with Stars"](https://docs.github.com/en/github/getting-started-with-github/saving-repositories-with-stars).

#### Seguir usuarios 
Puedes seguir a personas en GitHub para recibir notificaciones sobre su actividad y descubrir proyectos en sus comunidades. Cuando sigues a un usuario, su actividad pública en GitHub aparecerá en tu tablero para que puedas ver todas las cosas geniales en las que está trabajando.  
Para aprender más sobre seguir personas, lee ["Following People"](https://docs.github.com/en/github/getting-started-with-github/following-people).

#### Explorar con GitHub Explore 
GitHub Explore es un gran lugar para hacer justamente eso… explorar :smile:. Puedes encontrar proyectos nuevos, eventos y desarrolladores con quienes interactuar.

Puedes visitar el sitio de GitHub Explore [en github.com/explore](https://github.com/explore). Cuanto más interactúes con GitHub, más personalizado será tu Explore.

## 📝 Pasos opcionales siguientes 
* Abre un *pull request* y avísale a tu profesor(a) que terminaste este curso.  
* Crea un nuevo archivo Markdown en este repositorio. Cuéntales qué aprendiste y qué aún te genera dudas. ¡Experimenta con diferentes estilos!  
* Crea tu README de perfil. ¡Deja que el mundo sepa un poco más sobre ti! ¿Qué te interesa aprender? ¿En qué estás trabajando? ¿Cuál es tu pasatiempo favorito? Aprende más sobre cómo crear tu README de perfil en el documento ["Managing Your Profile README"](https://docs.github.com/en/github/setting-up-and-managing-your-github-profile/managing-your-profile-readme).  
* Ve a tu tablero de usuario y crea un nuevo repositorio. Experimenta con las funciones dentro de ese repositorio para familiarizarte con ellas.  
* [Cuéntanos qué te gustó o no te gustó del contenido de este curso](https://support.github.com/contact/education). ¿Qué te gustaría ver más? ¿Qué sería interesante o útil para tu camino de aprendizaje? 

## 📚  Recursos 
* [Un video corto que explica qué es GitHub](https://www.youtube.com/watch?v=w3jLJU7DT5E&feature=youtu.be)  
* [Recursos de aprendizaje de Git y GitHub](https://docs.github.com/en/github/getting-started-with-github/git-and-github-learning-resources)  
* [Entendiendo el flujo de GitHub](https://guides.github.com/introduction/flow/)  
* [Cómo usar ramas de GitHub](https://www.youtube.com/watch?v=H5GJfcp3p4Q&feature=youtu.be)  
* [Materiales interactivos de entrenamiento en Git](https://githubtraining.github.io/training-manual/#/01_getting_ready_for_class)  
* [Learning Lab de GitHub](https://lab.github.com/)  
* [Foro de la comunidad educativa](https://education.github.community/)  
* [Foro de la comunidad de GitHub](https://github.community/)  




