# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

### 5.1.1. Software Development Environment Configuration

**Project Management:**

WhatsApp (SaaS/Application): Aplicación de mensajería instantánea utilizada por el equipo para coordinar actividades, resolver dudas y mantener comunicación continua durante el desarrollo del proyecto. Ruta: https://www.whatsapp.com/ 

Trello (SaaS/Application): Herramienta de gestión de proyectos basada en la metodología Kanban, utilizada por el equipo para planificar, organizar y dar seguimiento al avance de las tareas del proyecto. A través de tableros, listas y tarjetas, se controlaron los sprints y se documentaron los entregables de cada fase. 
Ruta: https://trello.com/

**Product UX/UI design:**

Figma (SaaS/Application): Plataforma colaborativa en línea empleada para diseñar la interfaz visual del producto, diseñar Wireframes, crear prototipos interactivos y definir la estructura gráfica del sistema. Ruta: https://www.figma.com/ 

 
LucidChart (SaaS): Herramienta utilizada para crear user flows, representando visualmente las rutas y acciones que siguen los usuarios dentro del producto digital. Ruta: https://www.lucidchart.com/ 
 
**Software Development:**
Visual Studio Code (Application): Editor de código fuente multiplataforma que permite escribir, depurar y ejecutar el código del sistema. Incluye integración con GitHub para control de versiones. Ruta: https://code.visualstudio.com/ 

Live Preview (Extensión de Visual Studio Code) (Instalable): Extensión oficial de Microsoft que permite visualizar en tiempo real los cambios realizados en el código HTML, CSS y JavaScript dentro del navegador, facilitando el desarrollo web. Ruta: https://code.visualstudio.com/ 

 
GitHub (SaaS): Plataforma basada en Git utilizada para alojar repositorios de código, realizar control de versiones, seguimiento de cambios y trabajo colaborativo entre desarrolladores. Ruta: https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server

 
Software Testing:
Google Chrome (Application): Navegador web utilizado para realizar pruebas funcionales y de interfaz del producto digital, verificando el comportamiento y la visualización. Ruta: https://www.google.com/chrome 

**Software Documentation:**

**Markdown (Lenguaje de marcado ligero):** Utilizado para elaborar y mantener la documentación del proyecto de forma simple, legible y compatible con múltiples plataformas.  
  **Ruta:** https://www.markdownguide.org/


### 5.1.2. Source Code Management

El proyecto se gestionará mediante Git como sistema de control de versiones, utilizando el modelo de ramas GitFlow, propuesto por Vincent Driessen (2010), como workflow principal. Este modelo permite mantener una estructura ordenada y colaborativa para el desarrollo, pruebas y liberación del producto digital.
URL de repositorio de GitHub: https://github.com/GreeenMinds/EcoMind_LandingPage

**Estructura de Ramas (branches):**

**Ramas principales:**
•	Main: Versión estable y lista para producción
•	Develop: Rama de integración, se unirán todas las funcionalidades desarrolladas antes de preparar una versión oficial

**Ramas de soporte:**
•	Feature: Cada nueva funcionalidad o mejora se desarrollará en una rama independiente a partir de develop.
Convención de nombre: feature/nombre-descriptivo.
•	Release: Ramas temporales creadas desde develop para preparar una nueva versión antes de su lanzamiento. Solo se aplican correcciones menores o ajustes.
Convención de nombres: release/vX.Y.Z
•	Hotfix: Ramas utilizadas para solucionar errores críticos detectados en la versión de producción. Una vez corregido, se fusiona tanto en main como en develop.
Convención de nombres: hotfix/v.X.Y.Z

**Semantic Versioning:**
Se usará Semantic Versioning 2.0.0, utilizando el formato: MAJOR.MINOR.PATCH
MAJOR: Cambio incompatible
MINOR: Nueva funcionalidad compatible
PATCH: Corrección y ajuste menor

**Conventional Commits:**
Para los mensajes de commit se utilizará el estándar Conventional Commits, asegurando claridad y trazabilidad en el historial del proyecto. 

\<tipo>(\<opcional>): \<mensaje en presente>

Tipos:
•	feat: nueva funcionalidad.
•	fix: corrección de error.
•	docs: cambios en documentación.
•	style: formato o estilo (sin lógica).
•	refactor: reestructuración del código.
•	chore: tareas menores o de mantenimiento

### 5.1.3. Source Code Style Guide & Conventions

Para todos los lenguajes se aplicará la nomenclatura en inglés.

**Lenguaje HTML:** Se seguirá la guía HTML Style Guide and Coding Conventions y las recomendaciones de Google HTML/CSS Style Guide:

•	Los nombres de archivos serán en minúsculas, sin espacios, separados por guiones.
•	Las etiquetas estarán correctamente anidadas, en minúsculas y con sangría de dos espacios.
•	Los atributos HTML se escribirán en minúsculas y siempre entre comillas.
•	Los comentarios se usarán para describir secciones principales de código
•	Evitar largas líneas de código

**Lenguaje CSS:**
De acuerdo con Google HTML/CSS Style Guide:
•	Los nombres de clases y selectores se escribirán en minúsculas y con guiones (kebab-case).
•	Se mantendrá un orden lógico: primero estructura general, luego estilos específicos.
•	Se evitará el uso de estilos en línea dentro del HTML.
•	Los valores numéricos de cero no incluirán unidad.

**Lenguaje JavaScript:** Se seguirán las convenciones estándar de JavaScript Style Guide (Google y MDN):
•	Uso de camelCase para variables y funciones.
•	Uso de PascalCase para nombres de clases o constructores.
•	Uso de const y let en lugar de var.
•	Sangría de dos espacios y punto y coma al final de cada instrucción.
•	Los comentarios se harán con // para líneas simples o /* ... */ para bloques.

### 5.1.4. Software Deployment Configuration

Landing Page
El despliegue se realizará mediante GitHub Pages, una plataforma gratuita de GitHub que permite publicar sitios web estáticos directamente desde el repositorio de código fuente, sin necesidad de configurar servidores adicionales.
Procedimiento planificado:
1.	Verificar que la versión final del proyecto esté almacenada y actualizada en la rama main del repositorio.
2.	Acceder al repositorio en GitHub y dirigirse a Settings -> Pages.
3.	En la sección Source, seleccionar la rama main y la carpeta raíz.
4.	Guardar la configuración para que GitHub Pages genere automáticamente la página pública.
5.	Una vez desplegado, el sitio estará disponible.
Cuando el proyecto esté en fase de mantenimiento, las actualizaciones se gestionarán mediante commits y merges hacia la rama main. Cada cambio publicado en esta rama generará automáticamente una nueva versión desplegada del sitio.