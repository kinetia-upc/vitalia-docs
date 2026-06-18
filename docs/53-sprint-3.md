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
| **Sprint n Velocity** |  |
| **Sum of Story Points** |  |

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
      <td>AdrixRyz</td>
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
      <td>AdrixRyz</td>
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

#### *5.2.3.5. Execution Evidence for Sprint Review*

#### *5.2.3.6. Services Documentation Evidence for Sprint Review*

#### *5.2.3.7. Software Deployment Evidence for Sprint Review*

#### *5.2.3.8. Team Collaboration Insights during Sprint*
