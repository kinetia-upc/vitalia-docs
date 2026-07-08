### 5.2.4. Sprint 4

#### 5.2.4.1. Spring Planning 4

| **Sprint #** | 4 |
| --- | --- |
| **Date** | 2026-06-27 |
| **Time** | 20:00 |
| **Location** | Reunión virtual |
| **Prepared By** | Leo César Dulanto Espino |
| **Attendees** | Adrian Ruiz Mideyros, Nestor Alonso Rojas Tello, Alejandra Isabel Astocondor Bazan, Alexther Kamil Diaz Martinez, Leo César Dulanto Espino |
| **Sprint n Goal** | Our focus is on strengthening secure access, clinical continuity, and key integrations. We believe it delivers a more reliable experience to patients, doctors, and administrative staff. This will be confirmed when users can authenticate securely, recover access, preserve clinical data during connectivity issues, and complete exam, prescription, appointment, identity, and payment flows. |
| **Sprint n Velocity** | 50 sp |
| **Sum of Story Points** | 45 sp |

#### 5.2.4.2. Aspect Leaders and Collaborators

| Team Member | GitHub Username | Register/Login View | IAM API | Tenant | Pharmacy | Consume API |
| --- | --- | --- | --- | --- | --- | --- |
| Astocondor Bazan, Alejandra Isabel | AleeAsto | C | C | L | C | C |
| Dulanto Espino, Leo César | Leotens | C | L | C | C | C |
| Ruiz Mideyros, Adrian | AdrixRyz | C | C | C | C | L |
| Alexther Kamil Diaz Martinez | kamil-tron | L | C | C | C | C |
| Rojas Tello, Nestor Alonso | nes-ro | C | C | C | L | C |

#### 5.2.4.3. Sprint Backlog 4

**Trello Board Link:** [https://trello.com/invite/b/69e0ffa8dc72e4967311e1aa/ATTI47d8e7ca896972d7014ef7746935492a02062707/vitalia-board](https://trello.com/invite/b/69e0ffa8dc72e4967311e1aa/ATTI47d8e7ca896972d7014ef7746935492a02062707/vitalia-board)

<img src="../assets/images/others/s4-sprint-backlog.png" alt="Sprint Backlog 4" style="width: 100vw;">

Sprint #: Sprint 4

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
      <td>US002</td>
      <td>Inicio de sesión de usuario</td>
      <td>3</td>
      <td>TO60</td>
      <td>Vista de inicio de sesión</td>
      <td>Adaptar la pantalla de login para permitir el acceso de pacientes, doctores y administradores</td>
      <td>1</td>
      <td>kamil-tron</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US002</td>
      <td>Inicio de sesión de usuario</td>
      <td>3</td>
      <td>TO61</td>
      <td>Autenticación por rol</td>
      <td>Implementar validación de credenciales y respuesta con el rol correspondiente del usuario</td>
      <td>2</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US002</td>
      <td>Inicio de sesión de usuario</td>
      <td>3</td>
      <td>TO62</td>
      <td>Redirección por perfil</td>
      <td>Conectar el login con la navegación hacia el panel correspondiente según el rol autenticado</td>
      <td>1</td>
      <td>kamil-tron</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US035</td>
      <td>Cifrado de información médica sensible</td>
      <td>5</td>
      <td>TO63</td>
      <td>Reglas de cifrado clínico</td>
      <td>Definir los datos sensibles que deben protegerse en historias clínicas, diagnósticos y notas médicas</td>
      <td>2</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US035</td>
      <td>Cifrado de información médica sensible</td>
      <td>5</td>
      <td>TO64</td>
      <td>Cifrado en persistencia</td>
      <td>Implementar el almacenamiento protegido de información médica sensible antes de guardar registros</td>
      <td>2</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US035</td>
      <td>Cifrado de información médica sensible</td>
      <td>5</td>
      <td>TO65</td>
      <td>Validación de lectura segura</td>
      <td>Verificar que la información clínica cifrada pueda consultarse únicamente desde flujos autorizados</td>
      <td>1</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US036</td>
      <td>Bloqueos automáticos y sesiones seguras</td>
      <td>3</td>
      <td>TO66</td>
      <td>Temporizador de inactividad</td>
      <td>Implementar el cierre automático de sesión cuando el usuario permanece inactivo</td>
      <td>1</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US036</td>
      <td>Bloqueos automáticos y sesiones seguras</td>
      <td>3</td>
      <td>TO67</td>
      <td>Bloqueo por intentos fallidos</td>
      <td>Agregar control de intentos fallidos para impedir accesos indebidos reiterados</td>
      <td>1</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US036</td>
      <td>Bloqueos automáticos y sesiones seguras</td>
      <td>3</td>
      <td>TO68</td>
      <td>Mensaje de sesión expirada</td>
      <td>Mostrar una notificación clara al redirigir al usuario hacia el login por seguridad</td>
      <td>1</td>
      <td>Leotens</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US033</td>
      <td>Recuperación de contraseña</td>
      <td>3</td>
      <td>TO69</td>
      <td>Formulario de recuperación</td>
      <td>Construir la vista para solicitar recuperación de contraseña mediante correo o identificador</td>
      <td>1</td>
      <td>kamil-tron</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US033</td>
      <td>Recuperación de contraseña</td>
      <td>3</td>
      <td>TO70</td>
      <td>Token de restablecimiento</td>
      <td>Implementar generación y validación de tokens temporales para restablecer credenciales</td>
      <td>2</td>
      <td>kamil-tron</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US033</td>
      <td>Recuperación de contraseña</td>
      <td>3</td>
      <td>TO71</td>
      <td>Actualización de contraseña</td>
      <td>Conectar el flujo de nueva contraseña con la API de identidad y mensajes de confirmación</td>
      <td>1</td>
      <td>kamil-tron</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US029</td>
      <td>Integración con servicios de identidad (RENIEC)</td>
      <td>5</td>
      <td>TO72</td>
      <td>Consulta por DNI</td>
      <td>Implementar el servicio para consultar datos de identidad del paciente a partir de su DNI</td>
      <td>2</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US029</td>
      <td>Integración con servicios de identidad (RENIEC)</td>
      <td>5</td>
      <td>TO73</td>
      <td>Autocompletado de paciente</td>
      <td>Rellenar automáticamente nombres y apellidos en el registro administrativo de pacientes</td>
      <td>1</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US029</td>
      <td>Integración con servicios de identidad (RENIEC)</td>
      <td>5</td>
      <td>TO74</td>
      <td>Manejo de respuesta externa</td>
      <td>Validar respuestas exitosas, errores y documentos no encontrados desde el servicio de identidad</td>
      <td>1</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US030</td>
      <td>Sincronización con pasarelas de pago</td>
      <td>3</td>
      <td>TO75</td>
      <td>Registro de transacción externa</td>
      <td>Crear la estructura para almacenar identificadores, montos y estados de pagos digitales</td>
      <td>1</td>
      <td>AdrixRyz</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US030</td>
      <td>Sincronización con pasarelas de pago</td>
      <td>3</td>
      <td>TO76</td>
      <td>Validación de callback</td>
      <td>Procesar la respuesta de la pasarela para confirmar pagos y actualizar el estado financiero</td>
      <td>2</td>
      <td>AdrixRyz</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US030</td>
      <td>Sincronización con pasarelas de pago</td>
      <td>3</td>
      <td>TO77</td>
      <td>Conciliación visual</td>
      <td>Mostrar en la interfaz el resultado de la conciliación de pagos asociados a citas</td>
      <td>1</td>
      <td>AdrixRyz</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US014</td>
      <td>Solicitud de exámenes</td>
      <td>5</td>
      <td>TO78</td>
      <td>Modelo de orden de examen</td>
      <td>Definir la estructura de datos para registrar exámenes solicitados durante la consulta</td>
      <td>2</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US014</td>
      <td>Solicitud de exámenes</td>
      <td>5</td>
      <td>TO79</td>
      <td>Formulario de solicitud</td>
      <td>Construir el flujo para seleccionar exámenes y registrar la justificación clínica mínima</td>
      <td>1</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US014</td>
      <td>Solicitud de exámenes</td>
      <td>5</td>
      <td>TO80</td>
      <td>API de órdenes médicas</td>
      <td>Conectar el formulario con los servicios backend para crear y consultar órdenes de examen</td>
      <td>2</td>
      <td>AleeAsto</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US028</td>
      <td>Gestión de farmacia</td>
      <td>5</td>
      <td>TO81</td>
      <td>Listado de recetas emitidas</td>
      <td>Implementar la consulta de recetas disponibles para el seguimiento desde farmacia</td>
      <td>1</td>
      <td>nes-ro</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US028</td>
      <td>Gestión de farmacia</td>
      <td>5</td>
      <td>TO82</td>
      <td>Estado de dispensación</td>
      <td>Agregar actualización de estados para recetas pendientes, entregadas o observadas</td>
      <td>2</td>
      <td>nes-ro</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US028</td>
      <td>Gestión de farmacia</td>
      <td>5</td>
      <td>TO83</td>
      <td>Integración con inventario</td>
      <td>Relacionar la dispensación de recetas con la disponibilidad de medicamentos en farmacia</td>
      <td>2</td>
      <td>nes-ro</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US015</td>
      <td>Repetición rápida de recetas frecuentes</td>
      <td>5</td>
      <td>TO84</td>
      <td>Historial de recetas previas</td>
      <td>Mostrar recetas anteriores aptas para reutilización durante controles médicos</td>
      <td>1</td>
      <td>nes-ro</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US015</td>
      <td>Repetición rápida de recetas frecuentes</td>
      <td>5</td>
      <td>TO85</td>
      <td>Duplicación editable</td>
      <td>Permitir copiar medicamentos, dosis e indicaciones para revisión antes de emitir una nueva receta</td>
      <td>2</td>
      <td>nes-ro</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US015</td>
      <td>Repetición rápida de recetas frecuentes</td>
      <td>5</td>
      <td>TO86</td>
      <td>Restricciones de reutilización</td>
      <td>Validar que recetas restringidas o desactualizadas no puedan repetirse automáticamente</td>
      <td>1</td>
      <td>nes-ro</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US037</td>
      <td>Caché y guardado local temporal</td>
      <td>5</td>
      <td>TO87</td>
      <td>Detección de desconexión</td>
      <td>Identificar cortes de internet durante el registro de información clínica o administrativa</td>
      <td>1</td>
      <td>AdrixRyz</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US037</td>
      <td>Caché y guardado local temporal</td>
      <td>5</td>
      <td>TO88</td>
      <td>Guardado temporal local</td>
      <td>Almacenar temporalmente datos ingresados en LocalStorage o IndexedDB ante pérdida de conexión</td>
      <td>2</td>
      <td>AdrixRyz</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US037</td>
      <td>Caché y guardado local temporal</td>
      <td>5</td>
      <td>TO89</td>
      <td>Indicador de respaldo</td>
      <td>Mostrar al usuario que la información fue protegida temporalmente mientras no hay conexión</td>
      <td>1</td>
      <td>AdrixRyz</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US038</td>
      <td>Sincronización diferida tras restablecimiento</td>
      <td>3</td>
      <td>TO90</td>
      <td>Cola de sincronización</td>
      <td>Preparar una cola local de cambios pendientes para enviarlos cuando vuelva la conexión</td>
      <td>2</td>
      <td>kamil-tron</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US038</td>
      <td>Sincronización diferida tras restablecimiento</td>
      <td>3</td>
      <td>TO91</td>
      <td>Sincronización automática</td>
      <td>Enviar los datos pendientes al backend cuando el sistema detecte conectividad restablecida</td>
      <td>2</td>
      <td>kamil-tron</td>
      <td>Completed</td>
    </tr>
    <tr>
      <td>US038</td>
      <td>Sincronización diferida tras restablecimiento</td>
      <td>3</td>
      <td>TO92</td>
      <td>Confirmación de sincronización</td>
      <td>Informar al usuario que los datos guardados localmente fueron sincronizados correctamente</td>
      <td>1</td>
      <td>kamil-tron</td>
      <td>Completed</td>
    </tr>
  </tbody>
</table>

#### 5.2.4.4. Development Evidence for Sprint Review

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
      <td>0768b51</td>
      <td>feat: add sign up flow</td>
      <td>2026-07-02</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>develop</td>
      <td>0c59dc7</td>
      <td>feat: add sign in flow</td>
      <td>2026-07-02</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>develop</td>
      <td>007e709</td>
      <td>feat: add forgot password flow</td>
      <td>2026-07-02</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/IAM</td>
      <td>bb241c5</td>
      <td>feat: backend connection</td>
      <td>2026-07-02</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/IAM</td>
      <td>c12139c</td>
      <td>fix: dashboard connect</td>
      <td>2026-07-02</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/iam</td>
      <td>dbf931c</td>
      <td>feat: add iam module and extras</td>
      <td>2026-07-02</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>develop</td>
      <td>4ae13eb</td>
      <td>fix: many visual and backend connection bugs</td>
      <td>2026-07-03</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>a04b51f</td>
      <td>fix: several frontend modeling errors</td>
      <td>2026-07-03</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>develop</td>
      <td>5f5e4cf</td>
      <td>fix: deploy routing</td>
      <td>2026-07-04</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>develop</td>
      <td>b608145</td>
      <td>fix: patient flows bugs</td>
      <td>2026-07-04</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/cie10codes</td>
      <td>fadb433</td>
      <td>feat: add cie selector in clinic settings</td>
      <td>2026-07-04</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/cie10codes</td>
      <td>74d0411</td>
      <td>fix: improve medic attention workflow</td>
      <td>2026-07-04</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/cie10codes</td>
      <td>1cce686</td>
      <td>feat: add cie10diagnosis in doctor workflow</td>
      <td>2026-07-04</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>develop</td>
      <td>ccd03bd</td>
      <td>fix: save second diagnosis</td>
      <td>2026-07-04</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>7b0f5d2</td>
      <td>fix: patient flows bugs</td>
      <td>2026-07-04</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/cie10codes</td>
      <td>f87a7f4</td>
      <td>feat: add branch-based CIE-10 diagnosis catalog</td>
      <td>2026-07-04</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/cie10codes</td>
      <td>89c60fe</td>
      <td>fix: branch lookup for diagnosis catalog validation</td>
      <td>2026-07-04</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>0b9770d</td>
      <td>feat: WHO ICD-10 catalog provider</td>
      <td>2026-07-04</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>e035c1b</td>
      <td>feat: optimize database seeding</td>
      <td>2026-07-05</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>develop</td>
      <td>b30dfbf</td>
      <td>fix notification alert button, and schedule views</td>
      <td>2026-07-06</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>develop</td>
      <td>5017045</td>
      <td>Add MIT License to the project</td>
      <td>2026-07-06</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/tenant</td>
      <td>e734d35</td>
      <td>fix: CanConnect Function with Migrations</td>
      <td>2026-07-06</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/tenant</td>
      <td>611c1a8</td>
      <td>fix: CanConnect with Migrations, DB seeder ID generator, and add more availability slotes</td>
      <td>2026-07-06</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>1bef5a8</td>
      <td>Add MIT License to the project</td>
      <td>2026-07-06</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/fix_clinical</td>
      <td>958fb2a</td>
      <td>feat: update create user modal</td>
      <td>2026-07-07</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>develop</td>
      <td>75781db</td>
      <td>feat: Start attention before editing a medical record</td>
      <td>2026-07-07</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/tenant</td>
      <td>30f5e92</td>
      <td>fix: generate sequential medical record codes and stamp seed audit timestamps</td>
      <td>2026-07-07</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>develop</td>
      <td>226b614</td>
      <td>feat: improve doctor, patients views</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/fix_iam</td>
      <td>4717e86</td>
      <td>feat: register/iam with correct user</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/IAM</td>
      <td>f5db403</td>
      <td>feat:add weekly admissions date navigation</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/IAM</td>
      <td>5f68c0c</td>
      <td>feat:enhance admissions chart visuals</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/IAM</td>
      <td>2c89f9b</td>
      <td>feat:add admissions chart translations</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/IAM</td>
      <td>524d537</td>
      <td>feat:remove hardcoded operations labels</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/IAM</td>
      <td>5cd2780</td>
      <td>feat:improve operations board layout</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/IAM</td>
      <td>8914eca</td>
      <td>feat:fix availability slot deletion</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/fix-admin-view-create-user</td>
      <td>f119a21</td>
      <td>fix: fix admin update user modal</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/fix-admin-view-create-user</td>
      <td>3407073</td>
      <td>fix: persist role profile edits from admin users</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/IAM</td>
      <td>734418d</td>
      <td>feat: remove hardcoded system load metric</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/IAM</td>
      <td>252fd5c</td>
      <td>feat: refine billing revenue and claim resolution flow</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/IAM</td>
      <td>618f6a5</td>
      <td>feat: separate pharmacy catalog from branch inventory</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/IAM</td>
      <td>30f86e5</td>
      <td>feat: improve clinic settings pharmacy controls</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/scheduling</td>
      <td>51615db</td>
      <td>feat: extend prescription repository capabilities</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/scheduling</td>
      <td>c9a86db</td>
      <td>feat: update prescription and prescription detail command services</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/scheduling</td>
      <td>08cdb5a</td>
      <td>fix: minor adjustments to diagnosis, medical record and treatment services</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/scheduling</td>
      <td>176eea1</td>
      <td>feat: update database seeder</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/scheduling</td>
      <td>43ebece</td>
      <td>chore: update seed data</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/fix-admin-view-create-user</td>
      <td>80e1c86</td>
      <td>fix: allow optional password updates</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/fix-admin-view-create-user</td>
      <td>db60e80</td>
      <td>feat: add put doctor endpoint</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>develop</td>
      <td>5152211</td>
      <td>fix: Patients doctors view configuration</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/IAM</td>
      <td>8c6dd62</td>
      <td>feat: seed additional common medicines</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/IAM</td>
      <td>b155b24</td>
      <td>feat: expand pharmacy seed catalog</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/IAM</td>
      <td>853b86c</td>
      <td>fix: billing</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/healthcenter-register</td>
      <td>a7700ac</td>
      <td>feat: Add healthcare center selector to sign up</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/IAM</td>
      <td>76b0f7f</td>
      <td>fix: billing</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/doctor-dashboard-agenda-ui</td>
      <td>c28d4c2</td>
      <td>feat: doctor complete views</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/fix-billing-revenue-summary</td>
      <td>f260873</td>
      <td>fix: align billing revenue summary</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/healthcenter-register</td>
      <td>7aa5f87</td>
      <td>feat: add healthcare center selector to register</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/healthcenter-register</td>
      <td>c726a98</td>
      <td>fix: send normalized register payload</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/healthcenter-register</td>
      <td>b1b938c</td>
      <td>fix: keep admin-created role profiles linked</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/healthcenter-register</td>
      <td>c99fd36</td>
      <td>fix: improve register layout spacing</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/healthcenter-register</td>
      <td>3aa06f2</td>
      <td>feat: support healthcare center image url</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/healthcenter-register</td>
      <td>5040211</td>
      <td>fix: render sidebar healthcare center branding</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-frontend]</td>
      <td>feature/api-dni</td>
      <td>78dc441</td>
      <td>feat: add api peru</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/fix-swagger-documentation</td>
      <td>fae12a7</td>
      <td>feat: enforce jwt authentication</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/healthcenter-register</td>
      <td>209ef6a</td>
      <td>feat: add healthcare center image url</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/healthcenter-register</td>
      <td>40274ee</td>
      <td>feat: add healthcare center image url migration</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/healthcenter-register</td>
      <td>40274ee</td>
      <td>feat: add healthcare center image url migration</td>
      <td>2026-07-08</td>
    </tr>
    <tr>
      <td>[vitalia-backend]</td>
      <td>feature/healthcenter-register</td>
      <td>ef807d7</td>
      <td>feat: add endpoint IdentityLookup</td>
      <td>2026-07-08</td>
    </tr>
  </tbody>
</table>

#### 5.2.4.5. Execution Evidence for Sprint Review

#### 5.2.4.6. Services Documentation Evidence for Sprint Review

#### 5.2.4.7. Software Deployment Evidence for Sprint Review

Para este Sprint 4 no se requirió realizar un despliegue manual. Gracias a la configuración implementada en entregables previos, el proyecto ya cuenta con un flujo automatizado. De este modo, cualquier actualización o nuevo cambio integrado en la rama main desencadena automáticamente la actualización del despliegue en el entorno correspondiente.

**Landing Page link:** [https://kinetia-upc.github.io/vitalia-landing/](https://kinetia-upc.github.io/vitalia-landing/)

**Frontend link:** [https://vitalia-frontend-kinetia.vercel.app](https://vitalia-frontend-kinetia.vercel.app)

**Swagger Documentation Link:** [https://vitalia-backend-zf3p.onrender.com/swagger/index.html](https://vitalia-backend-zf3p.onrender.com/swagger/index.html)

**Landing page Deployment:**

<img src="../assets/images/others/s4-landing-deployment.png" alt="s4-landing-deploy" style="width: 100vw;"/>

**Frontend Deployment:**

<img src="../assets/images/others/s4-frontend-deployment.png" alt="s4-frontend-deploy" style="width: 100vw;"/>

**Backend Deployment:**

<img src="../assets/images/others/s4-backend-deployment.png" alt="s4-backend-deploy" style="width: 100vw;"/>

#### 5.2.4.8. Team Collaboration Insights during Sprint 

A continuación se presenta la evidencia de las interacciones y control de colaboración registrados durante el transcurso de este Sprint:

<img src="../assets/images/others/s4-collab-insight-front.png" alt="s4-collab-insight-front"  style="width: 100vw;"/>

<img src="../assets/images/others/s4-collab-insight-back.png" alt="s4-collab-insight-back" style="width: 100vw;"/>

El gráfico y métricas evidencian una alta frecuencia de commits organizados y un balance de responsabilidades alineado con los líderes técnicos de módulo definidos en la planificación.
