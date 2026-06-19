### 5.2.3. Sprint 3

#### *5.2.3.1. Sprint Planning 3*

| **Sprint #** | 3 |
| --- | --- |
| **Date** | 2026-06-07 |
| **Time** | 22:00 |
| **Location** | Reunión virtual |
| **Prepared By** | Adrian Ruiz Mideyros |
| **Attendees** | Adrian Ruiz Mideyros, Nestor Alonso Rojas Tello, Alejandra Isabel Astocondor Bazan, Alexther Kamil Diaz Martinez, Leo César Dulanto Espino |
| **Sprint n Goal** | Our focus is on establishing the core backend architecture and foundational APIs for secure user authentication and appointment workflows. We believe it delivers the automation and streamlining of clinical and administrative processes, ensuring a reliable and secure data flow to patients, doctors, and administrators. This will be confirmed when the frontend successfully authenticates users and retrieves real agenda data from the server, replacing the previously used mock APIs. |
| **Sprint n Velocity** | Designamos aceptar hasta 50 SP |
| **Sum of Story Points** | 48 SP |

#### *5.2.3.2. Aspect Leaders and Collaborators*

| Team Member | GitHub Username | Scheduling | Pharmacy | Clinical | Billing | Consume API |
| --- | --- | --- | --- | --- | --- | --- |
| Astocondor Bazan, Alejandra Isabel | AleeAsto | C | C | L | C | C |
| Dulanto Espino, Leo César | Leotens | L | C | C | C | C |
| Ruiz Mideyros, Adrian | AdrixRyz | C | C | C | C | L |
| Alexther Kamil Diaz Martinez | kamil-tron | C | L | C | C | C |
| Rojas Tello, Alonso | nes-ro | C | C | C | L | C |

#### *5.2.3.3. Sprint Backlog 3*

<p><strong>Sprint #:</strong> Sprint 3</p>

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
      <td>TS003</td>
      <td>Documentación OpenAPI/Swagger de endpoints</td>
      <td>3</td>
      <td>TO23</td>
      <td>Configuración de Swagger UI</td>
      <td>Integrar la documentación OpenAPI en el backend y habilitar Swagger UI</td>
      <td>2</td>
      <td>nes-ro</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>TS003</td>
      <td>Documentación OpenAPI/Swagger de endpoints</td>
      <td>3</td>
      <td>TO24</td>
      <td>Documentación de contratos REST</td>
      <td>Definir rutas, parámetros, cuerpos de solicitud y respuestas para los endpoints implementados</td>
      <td>2</td>
      <td>nes-ro</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>TS004</td>
      <td>Persistencia y repositorios por contexto</td>
      <td>5</td>
      <td>TO25</td>
      <td>Modelado de entidades backend</td>
      <td>Implementar entidades principales para Scheduling, Pharmacy, Clinical y Billing</td>
      <td>2</td>
      <td>AdrixRyz</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>TS004</td>
      <td>Persistencia y repositorios por contexto</td>
      <td>5</td>
      <td>TO26</td>
      <td>Repositorios y servicios de aplicación</td>
      <td>Crear repositorios y servicios para consultar, registrar y actualizar datos por bounded context</td>
      <td>2</td>
      <td>AdrixRyz</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US003</td>
      <td>Reserva digital de citas</td>
      <td>5</td>
      <td>TO27</td>
      <td>Endpoint de disponibilidad médica</td>
      <td>Implementar servicio para consultar horarios disponibles por especialidad, médico y fecha</td>
      <td>2</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US003</td>
      <td>Reserva digital de citas</td>
      <td>5</td>
      <td>TO28</td>
      <td>Endpoint de creación de citas</td>
      <td>Implementar registro de citas desde el backend y respuesta de confirmación para el frontend</td>
      <td>2</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US004</td>
      <td>Reprogramación de citas</td>
      <td>5</td>
      <td>TO29</td>
      <td>Validación de cambios de horario</td>
      <td>Implementar reglas para verificar disponibilidad y restricciones antes de reprogramar una cita</td>
      <td>2</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US004</td>
      <td>Reprogramación de citas</td>
      <td>5</td>
      <td>TO30</td>
      <td>Endpoint de reprogramación</td>
      <td>Actualizar fecha y hora de una cita existente y devolver la nueva programación al frontend</td>
      <td>2</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US005</td>
      <td>Cancelación de citas</td>
      <td>3</td>
      <td>TO31</td>
      <td>Reglas de cancelación</td>
      <td>Implementar validaciones para determinar si una cita puede ser cancelada</td>
      <td>1</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US005</td>
      <td>Cancelación de citas</td>
      <td>3</td>
      <td>TO32</td>
      <td>Endpoint de cancelación</td>
      <td>Actualizar el estado de la cita y liberar el horario correspondiente</td>
      <td>1</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US012</td>
      <td>Registro de anamnesis y examen físico</td>
      <td>5</td>
      <td>TO33</td>
      <td>Modelo de atención clínica</td>
      <td>Definir la estructura backend para registrar anamnesis, examen físico y observaciones clínicas</td>
      <td>2</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US012</td>
      <td>Registro de anamnesis y examen físico</td>
      <td>5</td>
      <td>TO34</td>
      <td>Endpoint de registro clínico</td>
      <td>Implementar guardado de la atención clínica asociada al paciente y médico responsable</td>
      <td>2</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US013</td>
      <td>Emisión de diagnóstico</td>
      <td>3</td>
      <td>TO35</td>
      <td>Entidad de diagnóstico</td>
      <td>Crear estructura para registrar diagnósticos vinculados a una atención clínica</td>
      <td>1</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US013</td>
      <td>Emisión de diagnóstico</td>
      <td>3</td>
      <td>TO36</td>
      <td>Endpoint de diagnóstico</td>
      <td>Implementar creación y consulta de diagnósticos desde el backend</td>
      <td>1</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US014</td>
      <td>Emisión de recetas digitales</td>
      <td>5</td>
      <td>TO37</td>
      <td>Modelo de receta digital</td>
      <td>Implementar estructura para medicamentos, dosis, frecuencia e indicaciones</td>
      <td>2</td>
      <td>kamil-tron</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US014</td>
      <td>Emisión de recetas digitales</td>
      <td>5</td>
      <td>TO38</td>
      <td>Endpoint de emisión de recetas</td>
      <td>Permitir la creación de recetas digitales asociadas a una atención clínica</td>
      <td>2</td>
      <td>kamil-tron</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US018</td>
      <td>Ingreso de medicinas al inventario</td>
      <td>3</td>
      <td>TO39</td>
      <td>Modelo de inventario farmacéutico</td>
      <td>Definir entidades para medicamentos, stock, presentación y disponibilidad</td>
      <td>1</td>
      <td>kamil-tron</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US018</td>
      <td>Ingreso de medicinas al inventario</td>
      <td>3</td>
      <td>TO40</td>
      <td>Endpoint de registro de medicinas</td>
      <td>Implementar creación y actualización de medicamentos desde el módulo de farmacia</td>
      <td>1</td>
      <td>kamil-tron</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US024</td>
      <td>Pagar la cita</td>
      <td>5</td>
      <td>TO41</td>
      <td>Modelo de pagos de citas</td>
      <td>Crear estructura para registrar montos, método de pago y estado de pago de una cita</td>
      <td>2</td>
      <td>nes-ro</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US024</td>
      <td>Pagar la cita</td>
      <td>5</td>
      <td>TO42</td>
      <td>Endpoint de pago</td>
      <td>Implementar registro de pago y actualización del estado financiero de la cita</td>
      <td>2</td>
      <td>nes-ro</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US026</td>
      <td>Control de pagos pendientes</td>
      <td>3</td>
      <td>TO43</td>
      <td>Consulta de pagos pendientes</td>
      <td>Implementar endpoint para listar atenciones y citas con pagos pendientes</td>
      <td>1</td>
      <td>nes-ro</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US026</td>
      <td>Control de pagos pendientes</td>
      <td>3</td>
      <td>TO44</td>
      <td>Filtros de seguimiento financiero</td>
      <td>Agregar filtros por estado, fecha y paciente para el seguimiento de cobros pendientes</td>
      <td>1</td>
      <td>nes-ro</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>TS005</td>
      <td>Integración del frontend con APIs reales</td>
      <td>5</td>
      <td>TO45</td>
      <td>Configuración de servicios HTTP reales</td>
      <td>Actualizar la capa de consumo del frontend para apuntar a los endpoints reales del backend</td>
      <td>2</td>
      <td>AdrixRyz</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>TS005</td>
      <td>Integración del frontend con APIs reales</td>
      <td>5</td>
      <td>TO46</td>
      <td>Reemplazo de mock services</td>
      <td>Sustituir llamadas al mock server por peticiones al backend en los módulos del Sprint 3</td>
      <td>2</td>
      <td>AdrixRyz</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>TS006</td>
      <td>Manejo de errores y validaciones API</td>
      <td>3</td>
      <td>TO47</td>
      <td>Validaciones de solicitudes</td>
      <td>Implementar validaciones para datos obligatorios, formatos y restricciones de negocio en los endpoints</td>
      <td>1</td>
      <td>AdrixRyz</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>TS006</td>
      <td>Manejo de errores y validaciones API</td>
      <td>3</td>
      <td>TO48</td>
      <td>Respuestas de error estandarizadas</td>
      <td>Definir códigos HTTP y mensajes de error consistentes para el consumo desde frontend</td>
      <td>1</td>
      <td>AdrixRyz</td>
      <td>Completed</td>
    </tr>
  </tbody>
</table>

#### *5.2.3.4. Development Evidence for Sprint Review*

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
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>ded9023</td>
      <td>feat: add initial structure</td>
      <td>2026-06-10</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>67a6ed8</td>
      <td>feat: add initial structure</td>
      <td>2026-06-10</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>5bac88b</td>
      <td>feat: Add bounded contexts initial structure</td>
      <td>2026-06-11</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>36c2453</td>
      <td>feat: Add bounded contexts initial structure</td>
      <td>2026-06-11</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/scheduling</td>
      <td>eacb780</td>
      <td>feat: add scheduling domain</td>
      <td>2026-06-14</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/scheduling</td>
      <td>c1e7702</td>
      <td>feat: add scheduling application</td>
      <td>2026-06-14</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/scheduling</td>
      <td>7f5e230</td>
      <td>feat: add scheduling infrastructure</td>
      <td>2026-06-14</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/scheduling</td>
      <td>1bcc553</td>
      <td>feat: add scheduling interfaces</td>
      <td>2026-06-14</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/scheduling</td>
      <td>811dd7a</td>
      <td>feat: Add scheduling resources</td>
      <td>2026-06-14</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/scheduling</td>
      <td>9b0dd39</td>
      <td>refactor: delete scheduling entities</td>
      <td>2026-06-14</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/scheduling</td>
      <td>52d06ee</td>
      <td>Merge pull request #2 from kinetia-upc/feature/scheduling</td>
      <td>2026-06-14</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/Pharmacy</td>
      <td>2149b5d</td>
      <td>feat: add pharmacy logic</td>
      <td>2026-06-15</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/Pharmacy</td>
      <td>a6e33d7</td>
      <td>Merge pull request #3 from kinetia-upc/feature/Pharmacy</td>
      <td>2026-06-15</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>0931c9e</td>
      <td>feat: configure database connection</td>
      <td>2026-06-16</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>476a264</td>
      <td>fix: Dockerfile config</td>
      <td>2026-06-16</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>598be83</td>
      <td>fix: init config</td>
      <td>2026-06-16</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/clinical</td>
      <td>fc660dc</td>
      <td>feat(clinical): add medical records endpoint</td>
      <td>2026-06-17</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/clinical</td>
      <td>dbf29c4</td>
      <td>feat(clinical): add diagnosis treatment and prescription endpoints</td>
      <td>2026-06-17</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/clinical</td>
      <td>f47adea</td>
      <td>feat(clinical): add medical record links and description updates</td>
      <td>2026-06-17</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/clinical</td>
      <td>82577cd</td>
      <td>feat(clinical): add business rules for clinical workflows</td>
      <td>2026-06-18</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/clinical</td>
      <td>468a8fe</td>
      <td>Merge pull request #4 from kinetia-upc/feature/clinical</td>
      <td>2026-06-18</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/billing</td>
      <td>502fe35</td>
      <td>feat: add context endpoints</td>
      <td>2026-06-18</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/billing</td>
      <td>30a1a2e</td>
      <td>feat: add context endpoints pt2</td>
      <td>2026-06-18</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/billing</td>
      <td>a250d12</td>
      <td>feat: Add billing bounded backend</td>
      <td>2026-06-18</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/billing</td>
      <td>24df5e2</td>
      <td>fix: date mistakes from frontend</td>
      <td>2026-06-18</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/billing</td>
      <td>e58f187</td>
      <td>Merge branch 'develop' into feature/billing</td>
      <td>2026-06-18</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/billing</td>
      <td>0cfbc28</td>
      <td>Merge pull request #5 from kinetia-upc/feature/billing</td>
      <td>2026-06-18</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>5c09bc4</td>
      <td>feat(clinical): implement get all endpoints for clinical resources to fix frontend 405 errors</td>
      <td>2026-06-18</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>6ea5a85</td>
      <td>refact: standardize error handling for pharmacy &amp; scheduling contexts and fix seeder</td>
      <td>2026-06-18</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>91eafc1</td>
      <td>fix: file copy mistake</td>
      <td>2026-06-18</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>46ebe7c</td>
      <td>fix: error handling</td>
      <td>2026-06-18</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>e7a5078</td>
      <td>fix: Swagger documentation</td>
      <td>2026-06-18</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/billing</td>
      <td>675e8b3</td>
      <td>Merge pull request #6 from kinetia-upc/feature/billing</td>
      <td>2026-06-18</td>
    </tr>
  </tbody>
</table>

#### *5.2.3.5. Execution Evidence for Sprint Review*

Durante el Sprint 3 se logró avanzar en la integración funcional entre el frontend y los servicios backend desarrollados para los principales flujos de Vitalia. Se implementaron y validaron vistas relacionadas con la gestión de citas, disponibilidad médica, atención clínica, diagnósticos, tratamientos, recetas digitales, medicamentos y reclamos de facturación, reemplazando progresivamente el uso de datos simulados por peticiones reales a la API. Las evidencias de ejecución presentadas en esta sección muestran las principales vistas implementadas y permiten comprobar que los usuarios pueden interactuar con funcionalidades clave del sistema dentro del alcance definido para el Sprint.

<img src="../assets/images/figures/Vitalia_Backend.png" alt="Vitalia_Backend" style="width: 100vw;">

#### *5.2.3.6. Services Documentation Evidence for Sprint Review*

Durante el Sprint 3 se documentaron los endpoints REST correspondientes a los contextos de Scheduling, Clinical, Pharmacy y Billing mediante OpenAPI/Swagger. Esta documentación permite evidenciar los servicios implementados dentro del alcance del Sprint, incluyendo las rutas base y las acciones disponibles para la gestion de citas, disponibilidad medica, registros clinicos, diagnosticos, recetas, tratamientos, medicamentos y reclamos de facturacion.

**Repositorio de Web Services:** [Repositorio backend de Vitalia](https://github.com/kinetia-upc/vitalia-backend)

**Repositorio Frontend:** [Repositorio frontend de Vitalia](https://github.com/kinetia-upc/vitalia-frontend)

**URL local de la documentación Swagger:** http://localhost:5032/swagger/index.html

**Base de datos utilizada:** MySQL

| Recurso             | Endpoint Base                                      | Acciones Implementadas                                     |
| ------------------- | -------------------------------------------------- | ---------------------------------------------------------- |
| Appointments | `/api/v1/appointments` | GET, POST, GET por ID, PATCH, DELETE |
| Availability Slots | `/api/v1/availabilitySlots` | GET, POST, GET por ID, PATCH, DELETE |
| Billing Claims | `/api/v1/billingClaims` | GET, POST, GET por ID, PUT, DELETE |
| Clinical Diagnoses | `/api/v1/diagnoses` | GET, POST, GET por ID, PATCH, DELETE, GET por medical record |
| Clinical Medical Records | `/api/v1/medicalRecords` | GET, POST, GET por code, GET por patient, GET por appointment |
| Clinical Prescription Details | `/api/v1/prescriptionDetails` | GET, POST, GET por ID, PUT, DELETE, GET por prescription |
| Clinical Prescriptions | `/api/v1/prescriptions` | GET, POST, GET por ID, DELETE, GET por medical record |
| Clinical Treatments | `/api/v1/treatments` | GET, POST, GET por ID, PATCH, DELETE, GET por medical record |
| Pharmacy Medicines | `/api/v1/medicines` | GET, POST, GET por ID, PUT, DELETE |

**Evidencia de ejecución**

Para mostrar la interación, ejecutamos 5 endpoints relacionados al bounded de scheduling. Entre los cuales veremos busqueda de citas y horarios disponibles, como su creación o eliminación de ellos.

1. GET /api/v1/appointments: Permite buscar citas, con parametros opcionales, los cuales van a filtrar segun indique el usuario. En esta ejecución no se añadio parametros, por lo cual nos brinda la lista completa de citas.

<img src="../assets/images/figures/Get_Appointments.png" alt="Get_Appointments Endpoint" style="width: 100vw;">

2. POST /api/v1/appointments: Se solicita la información necesaria para crear una cita. Al ejecutarse se añadira la cita a la base de datos.

<img src="../assets/images/figures/Post_Appointments.png" alt="Post_Appointments Endpoint" style="width: 100vw;">

3. GET /api/v1/availabilitySlots: Permite buscar horarios disponibles, con parametros opcionales, los cuales van a filtrar segun indique el usuario. En esta ejecución no se añadio parametros, por lo cual nos brinda la lista completa de horarios disponibles.

<img src="../assets/images/figures/Get_Availability_Slots.png" alt="Get_Availability_Slots Endpoint" style="width: 100vw;">

4. DELETE /api/v1/availabilitySlots: Da la posibilidad de eliminar un horario disponible de la base de datos. Para ello se solicita la id del horario que se desea eliminar. Tras su ejecución seria eliminado de la base de datos el horario asignado por la id.

<img src="../assets/images/figures/Delete_Availability_Slots.png" alt="Delete_Availability_Slots Endpoint" style="width: 100vw;">

5. GET /api/v1/availabilitySlots: Es el mismo endpoint de busqueda de horarios disponibles, en este caso lo volvemos a usar para verificar la eliminación del horario escogido (slot-003).

<img src="../assets/images/figures/Get_Availability_Slots_2.png" alt="Get_Availability_Slots_2 Endpoint" style="width: 100vw;">

#### *5.2.3.7. Software Deployment Evidence for Sprint Review*

#### *5.2.3.8. Team Collaboration Insights during Sprint*
