### 5.2.2. Sprint 2

#### *5.2.2.1. Sprint Planning 2*

Para el desarrollo del segundo sprint, el equipo se centrará en la construcción del Frontend de la aplicación web de Vitalia utilizando el framework Vue.js. El enfoque principal consiste en estructurar la arquitectura SPA (Single Page Application) utilizando herramientas como Vue Router y Pinia para la gestión de estados, implementar el sistema de diseño responsivo "Santuario Clínico" y simular/consumir datos (Fake API / json-server) para dar soporte a los flujos funcionales de pacientes, médicos y administradores.

| **Sprint #** | 2 |
| --- | --- |
| **Date** | 2026-05-10 |
| **Time** | 16:30 |
| **Location** | Reunión virtual |
| **Prepared By** | Nestor Alonso Rojas Tello |
| **Attendees** | Adrian Ruiz Mideyros, Nestor Alonso Rojas Tello, Alejandra Isabel Astocondor Bazan, Alexther Kamil Diaz Martinez, Leo César Dulanto Espino |
| **Sprint n Goal** | Our focus is on building a fully interactive and responsive user interface for the Vitalia web application using Vue.js. The goal is to implement secure Role-Based Access Control (RBAC) navigation, core patient workflows, and primary views for medical agendas and appointment booking, integrated with simulated data services (Mock APIs). This will be validated once the web application is deployed, ensuring a seamless, intuitive experience for patients, doctors, and administrators across both mobile and desktop devices. |
| **Sprint n Velocity** | Designamos aceptar hasta 34 SP |
| **Sum of Story Points** | 34 SP |

#### *5.2.2.2. Aspect Leaders and Collaborators*

| Team Member | GitHub Username | Vue Core & Router | Vistas Paciente | Vistas Médico | Vistas Admin | Mock Services |
| --- | --- | --- | --- | --- | --- | --- |
| Astocondor Bazan, Alejandra Isabel | AleeAsto | C | C | L | C | C |
| Dulanto Espino, Leo César | Leotens | C | C | C | L | C |
| Ruiz Mideyros, Adrian | AdrixRyz | L | C | C | C | C |
| Alexther Kamil Diaz Martinez | kamil-tron | C | L | C | C | C |
| Rojas Tello, Alonso | nes-ro | C | C | C | C | L |

#### *5.2.2.3. Sprint Backlog 2*

El Sprint Backlog 2 concentra la construcción del frontend principal de Vitalia, incluyendo la navegación, el diseño responsivo, el control de acceso por roles y los primeros flujos para pacientes, médicos y administradores. Con estas tareas se dejó una aplicación interactiva conectada a servicios simulados para validar la experiencia antes de integrar APIs reales.

**Trello Board Link:** [https://trello.com/invite/b/69e0ffa8dc72e4967311e1aa/ATTI47d8e7ca896972d7014ef7746935492a02062707/vitalia-board](https://trello.com/invite/b/69e0ffa8dc72e4967311e1aa/ATTI47d8e7ca896972d7014ef7746935492a02062707/vitalia-board)

<img src="../assets/images/others/s2-sprint-backlog.png" alt="Sprint Backlog 2" style="width: 100vw;">

<p><strong>Sprint #:</strong> Sprint 2</p>

<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th colspan="3">User Story</th>
      <th colspan="6">Work-Item / Task</th>
    </tr>
    <tr>
      <th>Id</th>
      <th>Title</th>
      <th>Story Points</th>
      <th>Id</th>
      <th>Title</th>
      <th>Description</th>
      <th>Estimation (Hours)</th>
      <th>Assigned To</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>US031</td>
      <td>Diseño responsive</td>
      <td>5</td>
      <td>TO13</td>
      <td>Componentes Base Responsivos</td>
      <td>Adaptar los layouts de UI "Santuario Clínico" a móvil/escritorio</td>
      <td>1</td>
      <td>AdrixRyz</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US039</td>
      <td>Navegación simple</td>
      <td>3</td>
      <td>TO14</td>
      <td>Configuración de Rutas y Sidebar</td>
      <td>Configurar el sistema de Vue Router y menú persistente</td>
      <td>1</td>
      <td>AdrixRyz</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US032</td>
      <td>Tiempo de respuesta ágil</td>
      <td>5</td>
      <td>TO15</td>
      <td>Lazy Loading y Componentes</td>
      <td>Implementar carga perezosa en rutas e imágenes pesadas</td>
      <td>1</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US008</td>
      <td>Accesibilidad de interfaz</td>
      <td>5</td>
      <td>TO16</td>
      <td>Ajustes de accesibilidad visual</td>
      <td>Mejorar legibilidad, jerarquía visual y claridad de acciones en las vistas principales</td>
      <td>1</td>
      <td>AdrixRyz</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US034</td>
      <td>Definición de accesos basados en roles (RBAC)</td>
      <td>5</td>
      <td>TO17</td>
      <td>Navigation Guards y Roles</td>
      <td>Implementar guards de navegación para restringir vistas</td>
      <td>1</td>
      <td>kamil-tron</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US001</td>
      <td>Registro de paciente</td>
      <td>5</td>
      <td>TO18</td>
      <td>Vista de Registro de Paciente</td>
      <td>Construir el formulario reactivo para nuevos pacientes</td>
      <td>1</td>
      <td>kamil-tron</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US006</td>
      <td>Consulta de historial clínico</td>
      <td>2</td>
      <td>TO19</td>
      <td>Panel de historial clínico</td>
      <td>Construir vista de historial del paciente</td>
      <td>1</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US007</td>
      <td>Consulta de resultados y recetas</td>
      <td>5</td>
      <td>TO20</td>
      <td>Vista de documentos clínicos</td>
      <td>Construir la visualización de resultados y recetas emitidas para el paciente</td>
      <td>1</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US027</td>
      <td>Descarga de historial clínico como PDF</td>
      <td>5</td>
      <td>TO21</td>
      <td>Descarga de historial</td>
      <td>Agregar acción para generar y descargar el historial clínico del paciente en formato PDF</td>
      <td>1</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US022</td>
      <td>Visualización de detalles de cita</td>
      <td>3</td>
      <td>TO22</td>
      <td>Detalle de cita del paciente</td>
      <td>Implementar la vista de detalle para consultar fecha, médico, especialidad y estado de una cita</td>
      <td>1</td>
      <td>kamil-tron</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US009</td>
      <td>Agenda médica diaria</td>
      <td>3</td>
      <td>TO23</td>
      <td>Calendario y Agenda</td>
      <td>Construir la visualización de la agenda médica</td>
      <td>1</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US021</td>
      <td>Visualización de mini calendario</td>
      <td>5</td>
      <td>TO24</td>
      <td>Mini calendario médico</td>
      <td>Agregar un calendario mensual para seleccionar días y revisar citas programadas</td>
      <td>1</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US010</td>
      <td>Consulta rápida del historial del paciente</td>
      <td>5</td>
      <td>TO25</td>
      <td>Acceso rápido a historial</td>
      <td>Implementar acceso al historial clínico del paciente desde el flujo de atención médica</td>
      <td>1</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US018</td>
      <td>Vista de HCE del paciente</td>
      <td>3</td>
      <td>TO26</td>
      <td>Vista HCE para médico</td>
      <td>Construir una vista resumida de historia clínica electrónica antes de la consulta</td>
      <td>1</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US016</td>
      <td>Gráficos evolutivos de visitas</td>
      <td>5</td>
      <td>TO27</td>
      <td>Gráficos de visitas</td>
      <td>Mostrar visualizaciones de tendencia de visitas del paciente en el módulo médico</td>
      <td>1</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US019</td>
      <td>Cierre de atención sin pérdida de datos</td>
      <td>5</td>
      <td>TO28</td>
      <td>Guardado confiable de atención</td>
      <td>Agregar confirmación de guardado y cierre seguro para la información registrada en consulta</td>
      <td>1</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US020</td>
      <td>Registro único de pacientes</td>
      <td>5</td>
      <td>TO29</td>
      <td>Registro administrativo de pacientes</td>
      <td>Implementar formulario administrativo para crear fichas únicas y evitar duplicidad de pacientes</td>
      <td>1</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US040</td>
      <td>Cancelar citas y eventos desde administración</td>
      <td>5</td>
      <td>TO30</td>
      <td>Cancelación administrativa</td>
      <td>Permitir al administrador cancelar citas o eventos registrados desde la agenda</td>
      <td>1</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US017</td>
      <td>Ingreso de medicinas al inventario</td>
      <td>2</td>
      <td>TO31</td>
      <td>Módulo de farmacia</td>
      <td>Implementar módulo de recetas y farmacia</td>
      <td>1</td>
      <td>nes-ro</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US024</td>
      <td>Facturación y cobros</td>
      <td>2</td>
      <td>TO32</td>
      <td>Vista de facturación</td>
      <td>Integrar métricas de facturación y pagos</td>
      <td>1</td>
      <td>nes-ro</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US026</td>
      <td>Dashboard operativo</td>
      <td>2</td>
      <td>TO33</td>
      <td>Tablero principal</td>
      <td>Implementar dashboard de administración</td>
      <td>1</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
  </tbody>
</table>

#### *5.2.2.4. Development Evidence for Sprint Review*

<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th>Repository</th>
      <th>Branch</th>
      <th>Commit Id</th>
      <th>Commit Message</th>      
      <th>Commited on (Date)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>develop</td>
      <td>356e2fa</td>
      <td>chore: setup initial project structure</td>
      <td>2026-05-10</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/clinical-context-foundation</td>
      <td>5e004eb</td>
      <td>feat(clinical): add domain entities, assemblers and api layer</td>
      <td>2026-05-11</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/scheduling</td>
      <td>a292493</td>
      <td>feat: Add scheduling entities and assemblers</td>
      <td>2026-05-11</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/medicalRecords</td>
      <td>1c00c0d</td>
      <td>fix(clinical): derive high priority from record signals</td>
      <td>2026-05-11</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/scheduling</td>
      <td>7137d8a</td>
      <td>feat: scheduling flow</td>
      <td>2026-05-12</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/patient-history</td>
      <td>bdc5f04</td>
      <td>feat: add patient history view</td>
      <td>2026-05-12</td>
    </tr><tr>
      <td>[vitalia-frontend]</td>
      <td>feature/pharmacy</td>
      <td>512456</td>
      <td>feat(pharmacy): add pharmacy context</td>
      <td>2026-05-12</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/profile-view</td>
      <td>59ca07a</td>
      <td>feat(profiles): add roles profiles</td>
      <td>2026-05-13</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/analytics</td>
      <td>035c0ed</td>
      <td>feat: add billing view</td>
      <td>2026-05-13</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/clinic-settings</td>
      <td>44d023f</td>
      <td>feat: add clinic settings view</td>
      <td>2026-05-13</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/admin-users-view</td>
      <td>875e0d4</td>
      <td>feat(admin): add admin users view</td>
      <td>2026-05-13</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/analytics</td>
      <td>2607f21</td>
      <td>feat(doctor): add doctor order view</td>
      <td>2026-05-13</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/scheduling</td>
      <td>7da4763</td>
      <td>feat: add functional calendar</td>
      <td>2026-05-13</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/billing</td>
      <td>c94073a</td>
      <td>feat: add payment in appointment</td>
      <td>2026-05-13</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/billing</td>
      <td>2e8520f</td>
      <td>feat: add prescriptions view</td>
      <td>2026-05-13</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/dashboard</td>
      <td>53144880</td>
      <td>feat: add dashboard flows</td>
      <td>2026-05-13</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/routes</td>
      <td>8fc2e5d</td>
      <td>feat: setup routes</td>
      <td>2026-05-13</td>
    </tr>
  </tbody>
</table>

#### *5.2.2.5. Execution Evidence for Sprint Review*

Durante este Sprint, el equipo completó con éxito la transición del diseño UI/UX hacia una aplicación interactiva construida en **Vue 3**. Se estructuró la arquitectura interna de la Single Page Application (SPA) y se integró la lógica de negocio en el Frontend mediante vistas reactivas para los tres perfiles de usuario (Administradores, Médicos y Pacientes).

**Principales entregables funcionales:**
- **Calendario y Flujo de Agendamiento:** Un calendario funcional que permite al paciente interactuar y programar citas médicas en tiempo real.
- **Historial Clínico Dinámico:** Un panel especializado que centraliza los antecedentes del paciente, facilitando la visualización rápida de registros médicos previos.
- **Módulo Administrativo y Facturación:** Tableros dedicados para la gestión de configuraciones de la clínica, perfiles de usuarios del sistema y analíticas/métricas de facturación iniciales.
- **Módulo de Farmacia y Órdenes Médicas:** Vistas diseñadas para el perfil del doctor enfocadas en la emisión estructurada de órdenes y seguimiento de recetas.

#### *5.2.2.6. Services Documentation Evidence for Sprint Review*

Para alimentar las vistas funcionales sin depender inicialmente de un backend de producción acoplado, el Frontend consume una **Fake API REST** desplegada independientemente. 

El diseño de la integración se organizó de la siguiente forma:
- **API Consumption Layer:** Módulos internos en Vue encargados de encapsular las peticiones HTTP (mediante Axios/Fetch) centralizando las llamadas hacia el servidor simulado.
- **Domain Entities & Assemblers:** Para mitigar riesgos de cambio de esquema, el proyecto implementa la capa de Entidades de Dominio y Ensambladores que transforman la respuesta cruda del JSON al modelo de datos de negocio de Vitalia.
- **Endpoint Simulation:** El mock server aloja colecciones clave como `/patients`, `/appointments`, `/medical-records`, `/pharmacy` y `/billing`.

#### *5.2.2.7. Software Deployment Evidence for Sprint Review*

El despliegue continuo del Frontend de la aplicación web (Single Page Application) se encuentra configurado exitosamente en Vercel.

**Frontend App Link:** [https://vitalia-frontend-kinetia.vercel.app](https://vitalia-frontend-kinetia.vercel.app)

<img src="../assets/images/others/s2-deployment-1.png" alt="s2-deployment-1" style="width: 100vw;"/>

<img src="../assets/images/others/s2-deployment-2.png" alt="s2-deployment-2" style="width: 100vw;"/>

#### *5.2.2.8. Team Collaboration Insights during Sprint*

Para la organización técnica del desarrollo del Frontend, el equipo adoptó un flujo de trabajo basado en GitFlow con ramas de características (`feature/`) bien definidas (como `feature/scheduling`, `feature/patient-history`, `feature/analytics`, etc.), garantizando una integración ordenada hacia la rama `develop`.

A continuación se presenta la evidencia de las interacciones y control de colaboración registrados durante el transcurso de este Sprint:

<img src="../assets/images/others/s2-collab-insight-1.png" alt="s2-collab-insight-1"  style="width: 100vw;"/>

<img src="../assets/images/others/s2-collab-insight-2.png" alt="s2-collab-insight-2" style="width: 100vw;"/>

El gráfico y métricas evidencian una alta frecuencia de commits organizados y un balance de responsabilidades alineado con los líderes técnicos de módulo definidos en la planificación.
