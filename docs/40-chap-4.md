# Capítulo IV: Product Design

## 4.1. Style Guidelines

### 4.1.1. General Style Guidelines

**Principios de diseño**

Vitalia es un SaaS integral diseñado para establecimientos de primer nivel de atención de salud. Su objetivo es centralizar la historia médica electrónica, citas y facturación, optimizando la gestión clínica. Por ello, nuestra estrella polar creativa es el "Santuario Clínico" (The Clinical Sanctuary).

Nos alejamos de las cuadrículas rígidas y estériles del software médico tradicional para adoptar una experiencia editorial de alta gama. El entorno debe sentirse autoritario pero calmado, sofisticado pero accesible.

- Profundidad Atmosférica: Utilizamos bases oscuras ("Pure Dark") superpuestas con superficies translúcidas. La interfaz debe sentirse como un instrumento físico premium.
- Claridad sobre el ruido: Rechazamos el aspecto de "plantilla" utilizando asimetría intencional, espacios en blanco generosos y una escala tipográfica de alto contraste que prioriza la legibilidad de los datos clínicos sin sacrificar la elegancia.

**Referencia Base y Adaptaciones**

El ecosistema visual toma como punto de partida **Material Design 3 (MD3)**, aprovechando sus paletas tonales para estructurar las elevaciones. Sin embargo, se han establecido reglas estrictas que modifican el sistema para adaptarlo a la identidad de Vitalia:

- Regla "No-Line": Queda estrictamente prohibido el uso de bordes sólidos de 1px para delimitar secciones o contenedores. Las fronteras estructurales se definen únicamente mediante cambios en el color de fondo (tonos de superficie).
- Sombras Ambientales (Ambient Shadows): Se evitan las sombras estándar. Las sombras se reservan para elementos flotantes y deben ser extremadamente difusas (ej. 0px 24px 48px rgba(0, 0, 0, 0.4) con un tinte sutil), imitando la luz ambiental natural.
- Efectos de Cristal (Glassmorphism): Los elementos flotantes o elevados utilizan fondos semitransparentes con desenfoque de fondo (backdrop-blur) para elevar la experiencia técnica.

**Paleta de Colores**

La paleta se rige por una filosofía "Pure Dark", reduciendo la fatiga visual del personal médico y permitiendo que la información crítica resalte a través de acentos luminosos.

- Primary (#20999E): Un cian médico luminoso y vibrante. Se reserva para acciones de alta prioridad, indicadores de estado activo (como en el menú lateral) y visualización de datos críticos.
- Secondary (#1A1F1F): Un azul oscuro como color de apoyo para elementos de la interfaz de usuario menos prominentes, chips y acciones secundarias.
- Tertiary (#C77646): Un tono albaricoque cálido, empleado para alertas de prioridad, notificaciones pendientes y acciones secundarias (ej. botón Logout), equilibrando los tonos fríos.
- Neutral Base (#121212): El lienzo principal del ecosistema. Refleja la profundidad de la plataforma y sostiene los demás elementos.

**Tipografía**

Se utiliza una estrategia de fuentes combinadas para equilibrar la precisión clínica con la estética. Nunca se usa blanco puro (#FFFFFF) para el texto principal; se emplea on_surface (ej. #e5e2e1) para cuidar la vista.

- Display & Headline (Manrope): Tipografía sans-serif geométrica con proporciones modernas. Su alta altura de la "x" transmite autoridad. Se usa para saludos iniciales, nombres de pacientes y métricas numéricas grandes.
- Body (Arimo): El caballo de batalla. Proporciona máxima legibilidad para registros médicos densos y tablas de datos.
- Label (Inter): Utilizada para metadatos (ej. fechas de última visita, IDs de pacientes) y etiquetas secundarias en color on_surface_variant para que pasen a un segundo plano, permitiendo que el dato principal resalte.

*Figura 17 (Color Palette & Tipography)*  
<img src="../assets/images/figures/19-color-palette.png" alt="Color Palette & Tipography" style="width: 100vw;">

**Componentes y Espaciado**

La profundidad en este sistema es un efecto atmosférico. Se imita la forma en que el papel fino reposa sobre un escritorio, sin sombras duras.

- Márgenes y Respiración: Se exige el uso de márgenes amplios (mínimo 32px) para permitir que los datos médicos respiren.
- Botones Principales: Forma de píldora (pill-shaped) máxima. Utilizan un relleno de gradiente sutil (de primary a primary_container) para los Calls to Action principales.
- Tarjetas Interactivas: Al pasar el cursor (hover), el fondo debe transicionar a una superficie más brillante (surface_bright) con una ligera elevación en el eje Y (0.25rem).
- Borde Fantasma (Ghost Border): Si un borde es estrictamente necesario por accesibilidad, se usará el token outline_variant a un máximo de 15% de opacidad.
- Componente "Vital Trace": Gráfico miniatura integrado en las tarjetas de pacientes. A diferencia de los gráficos tradicionales, este omite ejes o líneas de cuadrícula para priorizar la visualización rápida de tendencias. Utiliza un estilo de barras con relleno sólido en color primary para los datos recientes y opacidades reducidas para el histórico.

**Tono y Voz (Comunicación)**

El lenguaje utilizado en la plataforma debe reflejar la responsabilidad del entorno médico, transmitiendo confianza y reduciendo la carga de estrés del usuario.

| Dimensión | Espectro | Aplicación en el Diseño |
| --- | --- | --- |
| Divertido vs. Serio | Serio | La gestión de historias clínicas y facturación requiere rigor técnico. El tono serio transmite seguridad operativa y profesionalismo. |
| Formal vs. Casual | Formal | Mantenemos un estándar de comunicación propio de un entorno hospitalario de primer nivel, respetando títulos (ej. Dr. Vance). |
| Respetuoso vs. Irreverente | Respetuoso | La empatía es innegociable. Los mensajes de error, alertas de inventario o datos críticos de pacientes se comunican con tacto y claridad. |
| Entusiasta vs. Sereno | Sereno | El software actúa como un faro de calma. En momentos de alta carga laboral o emergencias médicas, la interfaz no abruma al usuario, sino que le ofrece control. |

### 4.1.2. Web Style Guidelines

Esta sección define cómo los principios visuales de Vitalia se adaptan fluidamente a través de diferentes dispositivos y tamaños de pantalla, garantizando que la experiencia de "Santuario Clínico" se mantenga intacta, accesible y ergonómica tanto en un monitor de escritorio como en una tablet clínica o un smartphone.

**Responsive Grid & Breakpoints**

El ecosistema utiliza un sistema de grilla fluida basada en columnas que se ajusta según el dispositivo, manteniendo siempre márgenes amplios para evitar la saturación visual de los datos médicos.

- Desktop (≥ 1024px): Grilla de 12 columnas. Márgenes exteriores amplios (mínimo 32px a 48px). Es el entorno principal donde se despliega toda la complejidad de la plataforma, permitiendo visualización lado a lado (ej. lista de pacientes y detalles simultáneos).
- Tablet / Clinical Screens (768px - 1023px): Grilla de 8 columnas. Márgenes exteriores de 24px. La interfaz se optimiza para el uso táctil en movimiento. Los módulos secundarios (como el panel de órdenes pendientes) pasan de estar en una columna lateral a apilarse debajo del contenido principal.
- Mobile (≤ 767px): Grilla de 4 columnas. Márgenes exteriores de 16px. Prioridad absoluta a la información crítica. El contenido se apila verticalmente al 100% del ancho.

**Adaptación de Layout y Navegación**

Para mantener la limpieza visual y el principio de "Profundidad Atmosférica", la navegación responde dinámicamente al espacio disponible:

- Desktop Navigation: El menú lateral (Sidebar) se mantiene fijo utilizando el token surface_container_lowest (#0e0e0e) para anclar el layout.
- Tablet & Mobile Navigation: El menú lateral se oculta y se transforma en un Drawer interactivo (menú hamburguesa) o en una Bottom Navigation Bar para acciones rápidas. Cuando el Drawer se abre, utiliza un fondo surface_container_low con una sombra ambiental difusa sobre el contenido principal oscurecido (Scrim al 40%).
- Manejo de Tablas de Datos: En pantallas pequeñas, las tablas clínicas complejas nunca deben colapsar rompiendo el texto. Se prioriza el uso de un contenedor con scroll horizontal (con un indicador visual sutil de sombra en el borde) o la transformación de cada fila en una "Tarjeta de Resumen" apilable.

**Estándares de Interacción (Interaction Patterns)**

Las interacciones deben sentirse precisas y responsivas, diferenciando claramente el comportamiento con mouse (escritorio) del comportamiento táctil (móvil/tablet).

**Estados Interactivos (Mouse vs. Touch)*+

- Hover (Solo Desktop): Al pasar el cursor sobre tarjetas interactivas (ej. Tarjetas de Pacientes), el fondo debe transicionar suavemente a surface_bright y aplicar una traslación en el eje Y (transform: translateY(-0.25rem)).
- Active / Pressed (Universal): Al hacer clic o tocar, el elemento reduce ligeramente su escala (transform: scale(0.98)) por 150ms para dar retroalimentación física. No se usan efectos de "hundimiento" con sombras.
- Focus (Teclado/Accesibilidad): Respetando la regla "No-Line", se elimina el anillo de enfoque azul nativo del navegador. En su lugar, los campos de entrada e inputs utilizan un resplandor de 2px en color primary (usando surface_tint al 30% de opacidad).
- Disabled (Inactivo): Los elementos deshabilitados reducen su opacidad al 38% y no responden a eventos de puntero o toque. Nunca cambian a escala de grises puros, mantienen la temperatura de la paleta oscura.

**Ergonomía y Touch Targets (Pantallas Táctiles)**

Dado que Vitalia puede usarse en entornos médicos de ritmo rápido (ej. tablets en consultorios):

- Área de Toque Mínima: Cualquier elemento interactivo (botones, íconos de menú, chips de estado) debe tener un área táctil invisible de al menos 48x48px, incluso si el elemento visual es más pequeño.
- Separación: Debe existir un mínimo de 8px entre áreas táctiles para prevenir toques accidentales en registros médicos o recetas.

**Responsive Typography & Hierarchy**

La tipografía se escala dinámicamente para asegurar que los datos no abrumen el espacio en pantallas pequeñas, pero sigan siendo legibles a un brazo de distancia.

- Fluid Scaling: Los tamaños de fuente, especialmente en títulos (display-lg, headline-md), se reducen en mobile. Por ejemplo, un dato crítico de 3.5rem en desktop bajará a 2.5rem en mobile.
- Body Text Intacto: El tamaño de la fuente de cuerpo (Public Sans para tablas e historias clínicas) nunca debe ser menor a 14px (0.875rem) en ningún dispositivo para garantizar la legibilidad sin necesidad de hacer zoom.
- Truncamiento Inteligente: En pantallas estrechas, los textos largos (como nombres completos o descripciones de diagnósticos) deben usar truncamiento con puntos suspensivos (text-overflow: ellipsis), asegurando que siempre haya un tooltip o acción táctil para ver la información completa.

**Adaptación de Componentes Clave**

- Modales y Diálogos: En Desktop, aparecen como ventanas flotantes centradas con Glassmorphism. En Mobile, se comportan como Bottom Sheets (hojas que suben desde la parte inferior de la pantalla) ocupando el 100% del ancho, facilitando el alcance del pulgar.
- Componente "Vital Trace": En resoluciones pequeñas, el gráfico miniatura de barras reducirá el número de barras visibles (mostrando solo las más recientes) antes de permitir que el componente se comprima demasiado y pierda su utilidad visual.

## 4.2. Information Architecture
La arquitectura de la información de Vitalia tiene como propósito principal estructurar, organizar y etiquetar el contenido de manera lógica y predecible. Las decisiones planteadas en esta sección están orientadas a garantizar que tanto los visitantes (en el Landing Page) como los usuarios de la clínica (en la Web Application) puedan adaptarse con fluidez a la plataforma, encontrando lo que necesitan sin esfuerzo cognitivo.

### 4.2.1. Organization Systems

Para estructurar los volúmenes de información de manera eficiente, Vitalia aplica una combinación de esquemas de organización visual y de categorización, adaptados al contexto del usuario.

**Esquemas de Organización Visual:**
* **Organización Jerárquica (Visual Hierarchy):** Utilizada en la Web Application. Existe un Dashboard principal que actúa como tronco, del cual se desprenden las ramas o módulos (Citas, Pacientes, Farmacia), terminando en las "hojas" o vistas de detalle (ej. el detalle de una consulta específica).
* **Organización Secuencial (Step-by-step):** Aplicada en procesos cerrados, como el *Booking Wizard* (donde el paciente elige especialidad $\rightarrow$ fecha $\rightarrow$ confirmación) y en el Landing Page para contar la historia del producto de forma progresiva.

**Esquemas de Categorización**

* **Según Audiencia (Grupos de Usuarios):** Utilizado en el Landing Page para segmentar el contenido mediante bloques específicos dirigidos a Médicos, Administradores y Pacientes, permitiendo que cada perfil identifique su propuesta de valor rápidamente.
* **Por Tópicos:** La navegación de la Web App agrupa las funciones según el dominio del negocio (ej. "Órdenes" agrupa laboratorio e imágenes; "Facturación" agrupa cobros, reportes de caja y liquidaciones).
* **Cronológico:** Aplicado de manera estricta dentro del módulo de Historia Clínica Electrónica (HCE) y la Agenda, organizando las atenciones, diagnósticos y reservas desde lo más reciente a lo más antiguo.

### 4.2.2. Labeling Systems

El sistema de etiquetado en Vitalia prioriza la simplicidad, buscando evitar la confusión técnica o médica en los pacientes, mientras mantiene el rigor profesional para el personal del policlínico. Se utilizan etiquetas cortas y representativas que asocian claramente el término con la funcionalidad esperada.

**Etiquetas para el Personal Médico y Administrativo (Profesional)**

| Etiqueta | Nivel de Organización | Significado / Asociación |
| --- | --- | --- |
| **Dashboard** | Módulo Principal | Panel de control con métricas rápidas del día y estado de la clínica. |
| **Agenda** | Módulo Principal | Calendario maestro de citas, bloqueos de horarios y consultorios. |
| **Patients** | Módulo Principal | Padrón demográfico e ingreso a la Historia Clínica Electrónica (HCE). |
| **Orders** | Módulo Secundario | Gestión de solicitudes y resultados de exámenes auxiliares (laboratorio). |
| **Billing** | Módulo Secundario | Gestión de comprobantes electrónicos, caja y liquidación de comisiones. |

**Etiquetas para los Pacientes (Simplificado y Personalizado)**

| Etiqueta | Nivel de Organización | Significado / Asociación |
| --- | --- | --- |
| **My Appointments** | Módulo Principal | Acceso directo para ver sus próximas visitas médicas o agendar una nueva. |
| **My History** | Módulo Principal | Su historial clínico resumido, diagnósticos pasados y antecedentes. |
| **Prescriptions** | Módulo Principal | Repositorio de recetas médicas digitales listas para su descarga. |
| **Settings** | Perfil de Usuario | Configuración de cuenta, preferencias de notificaciones y seguridad. |

### 4.2.3. SEO Tags and Meta Tags

Para asegurar la correcta indexación en motores de búsqueda y la presentación adecuada al compartir los enlaces, se han definido las siguientes etiquetas para las páginas de acceso público de la plataforma.

| Atributo | Landing Page (Comercial) | Web App (Login / Portal) |
| --- | --- | --- |
| **Title** | Vitalia by KinetiaLabs \| El SaaS Integral para Policlínicos | Vitalia App \| Iniciar Sesión |
| **Meta Description** | Centraliza tu policlínico: citas, historia clínica, farmacia y facturación en un solo sistema. Optimiza la gestión clínica de forma fácil y segura. | Accede a tu portal seguro en Vitalia. Gestiona tus citas médicas, revisa tus resultados y conéctate con tu clínica. |
| **Meta Keywords** | software para clinicas, historia clinica electronica peru, saas medico, gestion de policlinicos, facturacion medica, KinetiaLabs | vitalia login, portal del paciente, acceso medicos vitalia, historial clinico online |
| **Meta Author** | KinetiaLabs | KinetiaLabs |

### 4.2.4. Searching Systems

Vitalia procesa grandes volúmenes de datos diarios. Para evitar que los usuarios se sientan perdidos o abrumados, se ha implementado un sistema de búsqueda ubicuo y con filtros eficientes.

**Búsqueda Global (Médicos y Administradores)**

* **Opciones de búsqueda:** Barra persistente en la cabecera superior capaz de buscar por Nombre de Paciente, DNI o ID de cita.
* **Filtros:** Al interactuar con vistas de tablas (ej. Facturación), se activan filtros por rango de fechas, especialidad o estado (Completado/Pendiente).
* **Presentación de resultados:** La búsqueda principal utiliza un *auto-complete dropdown* que muestra resultados rápidos conforme el usuario escribe. Si se presiona "Enter", redirige a una lista estructurada y paginada con coincidencias exactas.

**Búsqueda para Pacientes**

* **Opciones de búsqueda:** Durante el flujo de reserva de citas, los pacientes cuentan con un buscador enfocado en Especialidades (ej. Cardiología) o Nombre del Médico.
* **Presentación de resultados:** Tarjetas visuales (Cards) del staff médico con su foto, disponibilidad más próxima y un botón directo de "Book Appointment".

### 4.2.5. Navigation Systems

El sistema de navegación define las acciones y técnicas que guían a los usuarios a través de la plataforma, asegurando que puedan cumplir sus metas de forma intuitiva. Se han diseñado dos sistemas paralelos según el producto:

**Navegación en Landing Page**

* **Sticky Header:** Barra de navegación superior fija que permite saltar mediante *anchor links* a las secciones de la página (Features, Segments, Pricing, Contact).
* **Call-to-Action (CTA):** Botones prominentes en color primario con el texto "Request a Demo" ubicados estratégicamente al inicio y al final del recorrido para guiar la conversión.

**Navegación en Web Application**

* **Left Sidebar Navigation:** Menú lateral fijo que aloja los módulos principales (Dashboard, Agenda, Patients, etc.). En dispositivos móviles (Mobile Web), este panel colapsa en un menú hamburguesa (Drawer) u ocupa una *Bottom Navigation Bar* para acciones frecuentes.
* **Breadcrumbs (Migas de Pan):** Utilizado en la parte superior del área de contenido para ubicar al usuario en niveles profundos. *Ejemplo: Patients > Javier Morales > Consultation 14/04*.
* **Profile Block:** Ubicado estáticamente en la parte inferior izquierda del Sidebar, consolidando el acceso a configuraciones de cuenta y desconexión segura sin ensuciar la navegación operativa.
## 4.3. Landing Page UI Design

### 4.3.1. Landing Page Wireframe

*Figura 20 (Landing Page Wireframe)*  
<img src="../assets/images/figures/20-landing-wireframe.png" alt="Landing Page Wireframe" style="width: 100vw;">

### 4.3.2. Landing Page Mock-up

*Figura 21 (Landing Page Mock-up)* 
<img src="../assets/images/figures/21-landing-mockup.png" alt="Landing Page Mock-Up" style="width: 100vw;">

## 4.4. Web Applications UX/UI Design

### 4.4.1. Web Applications Wireframes
*Figura 22 (Landing Page Mock-up)* 
<img src="../assets/images/figures/32-wirframeall.png" alt="32-wirframeall" style="width: 100vw;">

### 4.4.2. Web Applications Wireflow Diagrams

1. **Primer Segmento Objetivo (Administradores de establecimientos de PNAS)**

    - **Como** administrador de un establecimiento de PNAS, **quiero** registrar y mantener una ficha única de pacientes, **para** evitar duplicidades y asegurar que la información quede disponible para admisión, consultorio, laboratorio, farmacia y caja. (US021, US024)
    - **Como** administrador de un establecimiento de PNAS, **quiero** programar citas solicitadas por canales presenciales o telefónicos y confirmar la asistencia del paciente, **para** actualizar el flujo de atención en tiempo real. (US022, US023)
    - **Como** administrador de un establecimiento de PNAS, **quiero** gestionar el circuito operativo posterior a la atención, incluyendo recetas para farmacia, facturación electrónica y pagos pendientes, **para** mantener ordenado el proceso asistencial y financiero. (US025, US026, US029)
    - **Como** administrador de un establecimiento de PNAS, **quiero** consultar indicadores de citas, atenciones e ingresos en un dashboard, **para** tomar decisiones operativas con información consolidada y actualizada. (US027)
    - **Como** administrador de un establecimiento de PNAS, **quiero** generar reportes automáticos e integrar Vitalia con otros sistemas mediante API, **para** reducir trabajo manual y evitar el aislamiento de la operación del establecimiento. (US028, US030)

    *Figura 23 (Wireflow 1 Administradores)* 
    <img src="../assets/images/figures/23-Wireflow-Admin-1.png" alt="Landing Page Mock-Up" style="width: 100vw;">

    *Figura 24 (Wireflow 2 Administradores)* 
    <img src="../assets/images/figures/24-Wireflow-Admin-2.png" alt="Landing Page Mock-Up" style="width: 100vw;">

    *Figura 25 (Wireflow 3 Administradores)* 
    <img src="../assets/images/figures/25-Wireflow-Admin-3.png" alt="Landing Page Mock-Up" style="width: 100vw;">

    *Figura 26 (Wireflow 4 Administradores)* 
    <img src="../assets/images/figures/26-Wireflow-Admin-4.png" alt="Landing Page Mock-Up" style="width: 100vw;">

    *Figura 27 (Wireflow 5 Administradores)* 
    <img src="../assets/images/figures/27-Wireflow-Admin-5.png" alt="Landing Page Mock-Up" style="width: 100vw;">

2.  **Segundo Segmento Objetivo (Doctores de establecimientos de PNAS)**

    - **Como** doctor de un establecimiento de PNAS, **quiero** revisar mi agenda diaria, el estado de mis citas y los datos de triaje antes de la consulta, **para** preparar mejor cada atención. (US010, US019)
    - **Como** doctor de un establecimiento de PNAS, **quiero** acceder rápidamente al historial clínico y a un resumen automático del paciente, **para** tomar decisiones con antecedentes relevantes dentro del tiempo disponible. (US011, US017)
    - **Como** doctor de un establecimiento de PNAS, **quiero** registrar la anamnesis, el examen físico y el diagnóstico en una sola atención, **para** mantener la información clínica ordenada y completa. (US012, US013)
    - **Como** doctor de un establecimiento de PNAS, **quiero** emitir recetas digitales y órdenes de exámenes desde la misma consulta, **para** facilitar el tratamiento, la dispensación y el seguimiento diagnóstico del paciente. (US014, US015)

    *Figura 28 (Wireflow 1 Doctores)* 
    <img src="../assets/images/figures/28-Wireflow-Doctor-1.png" alt="Landing Page Mock-Up" style="width: 100vw;">

    *Figura 29 (Wireflow 2 Doctores)* 
    <img src="../assets/images/figures/29-Wireflow-Doctor-2.png" alt="Landing Page Mock-Up" style="width: 100vw;">

    *Figura 30 (Wireflow 3 Doctores)* 
    <img src="../assets/images/figures/30-Wireflow-Doctor-3.png" alt="Landing Page Mock-Up" style="width: 100vw;">

    *Figura 31 (Wireflow 4 Doctores)* 
    <img src="../assets/images/figures/31-Wireflow-Doctor-4.png" alt="Landing Page Mock-Up" style="width: 100vw;">

3. **Tercer Segmento Objetivo (Pacientes de todas las edades)**

    - **Como** paciente, **quiero** crear una cuenta e iniciar sesión de manera sencilla y segura, **para** acceder a mis servicios médicos desde un solo lugar. (US001, US002)
    - **Como** paciente, **quiero** reservar, reprogramar o cancelar citas digitales en pocos pasos, **para** adaptar mi atención a mi disponibilidad sin depender de llamadas o trámites presenciales. (US003, US004, US005)
    - **Como** paciente, **quiero** recibir recordatorios automáticos de mis citas, **para** reducir olvidos, inasistencias y confusiones sobre la fecha u hora de atención. (US008)
    - **Como** paciente, **quiero** consultar mi historial clínico, resultados y recetas emitidas en línea, **para** dar seguimiento a mis diagnósticos y tratamientos sin solicitar copias físicas. (US006, US007)

        *Figura 32 (Wireflow 1 Pacientes)* 
    <img src="../assets/images/figures/32-Wireflow-Pacient-1.png" alt="Landing Page Mock-Up" style="width: 100vw;">
    
        *Figura 33 (Wireflow 2 Pacientes)* 
    <img src="../assets/images/figures/33-Wireflow-Pacient-2.png" alt="Landing Page Mock-Up" style="width: 100vw;">
    
        *Figura 34 (Wireflow 3 Pacientes)* 
    <img src="../assets/images/figures/34-Wireflow-Pacient-3.png" alt="Landing Page Mock-Up" style="width: 100vw;">

        *Figura 35 (Wireflow 4 Pacientes)* 
    <img src="../assets/images/figures/35-Wireflow-Pacient-4.png" alt="Landing Page Mock-Up" style="width: 100vw;">

### 4.4.3. Web Applications Mock-ups

*Figura 36 (Admin Clinic Settings)*  
<img src="../assets/images/figures/36-Admin Clinic Settings.png" alt="36-Admin Clinic Settings" style="width: 100vw;">

*Figura 37 (Admin Billing)*  
<img src="../assets/images/figures/37-Admin Billing.png" alt="37-Admin Billing" style="width: 100vw;">

*Figura 38 (Admin Operations)*  
<img src="../assets/images/figures/38-Admin Operations.png" alt="38-Admin Operations" style="width: 100vw;">

*Figura 39 (Admin Users)*  
<img src="../assets/images/figures/39-Admin Users.png" alt="39-Admin Users" style="width: 100vw;">

*Figura 40 (Admin Dashboard)*  
<img src="../assets/images/figures/40-Admin Dashboard.png" alt="40-Admin Dashboard" style="width: 100vw;">

*Figura 41 (Patient Profile)*  
<img src="../assets/images/figures/41-Patient Profile.png" alt="41-Patient Profile" style="width: 100vw;">

*Figura 42 (Patient History)*  
<img src="../assets/images/figures/42-Patient History.png" alt="42-Patient History" style="width: 100vw;">

*Figura 43 (Patient Prescriptions)*  
<img src="../assets/images/figures/43-Patient Prescriptions.png" alt="43-Patient Prescriptions" style="width: 100vw;">

*Figura 44 (Patient Appointments)*  
<img src="../assets/images/figures/44-Patient Appointments.png" alt="44-Patient Appointments" style="width: 100vw;">

*Figura 45 (Patient Dashboard)*  
<img src="../assets/images/figures/45-Patient Dashboard.png" alt="45-Patient Dashboard" style="width: 100vw;">

*Figura 46 (Doctor Profile)*  
<img src="../assets/images/figures/46-Doctor Profile.png" alt="46-Doctor Profile" style="width: 100vw;">

*Figura 47 (Doctor Orders)*  
<img src="../assets/images/figures/47-Doctor Orders.png" alt="47-Doctor Orders" style="width: 100vw;">

*Figura 48 (Doctor Agenda)*  
<img src="../assets/images/figures/48-Doctor Agenda.png" alt="48-Doctor Agenda" style="width: 100vw;">

*Figura 49 (Doctor Patients)*  
<img src="../assets/images/figures/49-Doctor Patients.png" alt="49-Doctor Patients" style="width: 100vw;">

*Figura 50 (Doctor Dashboard)*  
<img src="../assets/images/figures/50-Doctor Dashboard.png" alt="50-Doctor Dashboard" style="width: 100vw;">



### 4.4.4. Web Applications User Flow Diagrams

1. **Primer Segmento Objetivo (Administradores de establecimientos de PNAS)**

    - **Como** administrador de un establecimiento de PNAS, **quiero** registrar y mantener una ficha única de pacientes, **para** evitar duplicidades y asegurar que la información quede disponible para admisión, consultorio, laboratorio, farmacia y caja. (US021, US024)
    - **Como** administrador de un establecimiento de PNAS, **quiero** programar citas solicitadas por canales presenciales o telefónicos y confirmar la asistencia del paciente, **para** actualizar el flujo de atención en tiempo real. (US022, US023)
    - **Como** administrador de un establecimiento de PNAS, **quiero** gestionar el circuito operativo posterior a la atención, incluyendo recetas para farmacia, facturación electrónica y pagos pendientes, **para** mantener ordenado el proceso asistencial y financiero. (US025, US026, US029)
    - **Como** administrador de un establecimiento de PNAS, **quiero** consultar indicadores de citas, atenciones e ingresos en un dashboard, **para** tomar decisiones operativas con información consolidada y actualizada. (US027)
    - **Como** administrador de un establecimiento de PNAS, **quiero** generar reportes automáticos e integrar Vitalia con otros sistemas mediante API, **para** reducir trabajo manual y evitar el aislamiento de la operación del establecimiento. (US028, US030)

    *Figura 51 (Userflow 1 Administradores)* 
    <img src="../assets/images/figures/51-Userflow-Admin-1.png" alt="Landing Page Mock-Up" style="width: 100vw;">

    *Figura 52 (Userflow 2 Administradores)* 
    <img src="../assets/images/figures/24-Userflow-Admin-2.png" alt="Landing Page Mock-Up" style="width: 100vw;">

    *Figura 53 (Userflow 3 Administradores)* 
    <img src="../assets/images/figures/53-Userflow-Admin-3.png" alt="Landing Page Mock-Up" style="width: 100vw;">

    *Figura 54 (Userflow 4 Administradores)* 
    <img src="../assets/images/figures/54-Userflow-Admin-4.png" alt="Landing Page Mock-Up" style="width: 100vw;">

    *Figura 55 (Userflow 5 Administradores)* 
    <img src="../assets/images/figures/55-Userflow-Admin-5.png" alt="Landing Page Mock-Up" style="width: 100vw;">

2.  **Segundo Segmento Objetivo (Doctores de establecimientos de PNAS)**

    - **Como** doctor de un establecimiento de PNAS, **quiero** revisar mi agenda diaria, el estado de mis citas y los datos de triaje antes de la consulta, **para** preparar mejor cada atención. (US010, US019)
    - **Como** doctor de un establecimiento de PNAS, **quiero** acceder rápidamente al historial clínico y a un resumen automático del paciente, **para** tomar decisiones con antecedentes relevantes dentro del tiempo disponible. (US011, US017)
    - **Como** doctor de un establecimiento de PNAS, **quiero** registrar la anamnesis, el examen físico y el diagnóstico en una sola atención, **para** mantener la información clínica ordenada y completa. (US012, US013)
    - **Como** doctor de un establecimiento de PNAS, **quiero** emitir recetas digitales y órdenes de exámenes desde la misma consulta, **para** facilitar el tratamiento, la dispensación y el seguimiento diagnóstico del paciente. (US014, US015)

    *Figura 56 (Userflow 1 Doctores)* 
    <img src="../assets/images/figures/56-Userflow-Doctor-1.png" alt="Landing Page Mock-Up" style="width: 100vw;">

    *Figura 57 (Userflow 2 Doctores)* 
    <img src="../assets/images/figures/57-Userflow-Doctor-2.png" alt="Landing Page Mock-Up" style="width: 100vw;">

    *Figura 58 (Userflow 3 Doctores)* 
    <img src="../assets/images/figures/58-Userflow-Doctor-3.png" alt="Landing Page Mock-Up" style="width: 100vw;">

    *Figura 59 (Userflow 4 Doctores)* 
    <img src="../assets/images/figures/59-Userflow-Doctor-4.png" alt="Landing Page Mock-Up" style="width: 100vw;">

3. **Tercer Segmento Objetivo (Pacientes de todas las edades)**

    - **Como** paciente, **quiero** crear una cuenta e iniciar sesión de manera sencilla y segura, **para** acceder a mis servicios médicos desde un solo lugar. (US001, US002)
    - **Como** paciente, **quiero** reservar, reprogramar o cancelar citas digitales en pocos pasos, **para** adaptar mi atención a mi disponibilidad sin depender de llamadas o trámites presenciales. (US003, US004, US005)
    - **Como** paciente, **quiero** recibir recordatorios automáticos de mis citas, **para** reducir olvidos, inasistencias y confusiones sobre la fecha u hora de atención. (US008)
    - **Como** paciente, **quiero** consultar mi historial clínico, resultados y recetas emitidas en línea, **para** dar seguimiento a mis diagnósticos y tratamientos sin solicitar copias físicas. (US006, US007)

    *Figura 60 (Userflow 1 Pacientes)* 
    <img src="../assets/images/figures/60-Userflow-Pacient-1.png" alt="Landing Page Mock-Up" style="width: 100vw;">
    
    *Figura 61 (Userflow 2 Pacientes)* 
    <img src="../assets/images/figures/61-Userflow-Pacient-2.png" alt="Landing Page Mock-Up" style="width: 100vw;">
    
    *Figura 62 (Userflow 3 Pacientes)* 
    <img src="../assets/images/figures/62-Userflow-Pacient-3.png" alt="Landing Page Mock-Up" style="width: 100vw;">

    *Figura 63 (Userflow 4 Pacientes)* 
    <img src="../assets/images/figures/63-Userflow-Pacient-4.png" alt="Landing Page Mock-Up" style="width: 100vw;">


## 4.5. Web Applications Prototyping



## 4.6. Domain-Driven Software Architecture

### 4.6.1. Design-Level EventStorming

Se utilizó la guía de Philippe Bourgau, proporcionada en la rúbrica del Final Problem Statement, para llevar a cabo el proceso de Design-Level EventStorming, con el objetivo de identificar los Bounded Contexts, siguiendo sus etapas:

- Unstructured Exploration
- Timelines
- Pain Points
- Pivotal Points
- Commands
- Policies
- Read Models
- External Systems
- Aggregates
- Bounded Contexts

Miro Board Link: https://miro.com/app/board/uXjVGhdfT5g=/?share_link_id=948975680057

*Figura XX (Design Level EventStorming)*  
<img src="../assets/images/figures/xx-design-level-event-storming.jpeg" alt="Design Level EventStorming" style="width: 100vw;">

### 4.6.2. Software Architecture Context Diagram

El diagrama de contexto presenta una visión de alto nivel del sistema Vitalia, mostrando su interacción con los actores externos y sistemas externos relevantes. Este diagrama permite comprender el alcance del sistema, identificando quiénes lo utilizan y con qué servicios externos se integra, sin entrar en detalles técnicos internos.

*Figura XX (Context Diagram)*  
<img src="../assets/images/figures/xx-context-diagram.png" alt="Design Level EventStorming" style="width: 100vw;">

### 4.6.3. Software Architecture Container Diagrams

El diagrama de contenedores descompone el sistema en sus principales unidades de ejecución, mostrando cómo se distribuyen las responsabilidades dentro de la arquitectura. En este nivel se identifican elementos como la aplicación web, API Gateway y los distintos servicios o bounded contexts, así como las tecnologías utilizadas y la forma en que estos se comunican entre sí.

*Figura XX (Container Diagram)*  
<img src="../assets/images/figures/xx-container-diagram.png" alt="Design Level EventStorming" style="width: 100vw;">

### 4.6.4. Software Architecture Components Diagrams

El diagrama de componentes profundiza en cada contenedor, detallando los módulos internos que lo conforman y sus interacciones. Este nivel permite visualizar la organización interna.

*Figura XX (Component Diagram - Identity & Tenant Context)*  
<img src="../assets/images/figures/xx-component-diagram-1.png" alt="Design Level EventStorming" style="width: 100vw;">

*Figura XX (Component Diagram - Clinical Context)*  
<img src="../assets/images/figures/xx-component-diagram-2.png" alt="Design Level EventStorming" style="width: 100vw;">

*Figura XX (Component Diagram - Schedule Context)*  
<img src="../assets/images/figures/xx-component-diagram-3.png" alt="Design Level EventStorming" style="width: 100vw;">

*Figura XX (Component Diagram - Pharmacy & Inventory Context)*  
<img src="../assets/images/figures/xx-component-diagram-4.png" alt="Design Level EventStorming" style="width: 100vw;">

*Figura XX (Component Diagram - Dashboard and Analytics Context)*  
<img src="../assets/images/figures/xx-component-diagram-5.png" alt="Design Level EventStorming" style="width: 100vw;">

*Figura XX (Component Diagram - Billing Context)*  
<img src="../assets/images/figures/xx-component-diagram-6.png" alt="Design Level EventStorming" style="width: 100vw;">

## 4.7. Software Object-Oriented Design

### 4.7.1. Class Diagrams

En la primera etapa, se elaboró el diagrama de clases general identificando las principales entidades del dominio de Vitalia, así como sus atributos, métodos, relaciones y multiplicidades. Este paso permitió establecer una visión global del sistema, asegurando que todos los elementos relevantes del negocio estuvieran correctamente modelados y conectados entre sí.

En la segunda etapa, estas clases fueron organizadas en distintos Bounded Context, agrupándolas según su responsabilidad, propósito y cohesión dentro del sistema. Esta separación permitió delimitar claramente los contextos del dominio, facilitando la comprensión del sistema y reduciendo la complejidad al dividirlo en módulos más manejables, alineados con la lógica de negocio.

Finalmente, en la tercera etapa, se realizó un análisis más profundo de cada clase dentro de su contexto, clasificándolas como Entity, Value Object o Aggregate. Esta identificación permitió definir con precisión las reglas de negocio, los límites de consistencia y las responsabilidades de cada componente dentro del dominio. Como resultado, los diagramas finales reflejan una arquitectura sólida, coherente y alineada con los principios de DDD, mostrando no solo la estructura del sistema, sino también la lógica y comportamiento del dominio.

*Figura XX (Class Diagram - Identity and Clinic Context)*  
<img src="../assets/diagrams/class-diagram-etapa-3-identity-clinic-context.svg" alt="Class Diagram - Identity and Clinic Context" style="width: 100vw;">

*Figura XX (Class Diagram - Clinical Context)*  
<img src="../assets/diagrams/class-diagram-etapa-3-clinical-context.svg" alt="Class Diagram - Clinical Context" style="width: 100vw;">

*Figura XX (Class Diagram - Scheduling Context)*  
<img src="../assets/diagrams/class-diagram-etapa-3-scheduling-context.svg" alt="Class Diagram - Scheduling Context" style="width: 100vw;">

*Figura XX (Class Diagram - Pharmacy & Inventory Context)*  
<img src="../assets/diagrams/class-diagram-etapa-3-pharmacy-inventory-context.svg" alt="Class Diagram - Pharmacy and Inventory Context" style="width: 100vw;">

*Figura XX (Class Diagram - Dashboard and Analytics Context)*  
<img src="../assets/diagrams/class-diagram-etapa-3-dashboard-analytics-context.svg" alt="Class Diagram - Dashboard and Analytics Context" style="width: 100vw;">

*Figura XX (Class Diagram - Billing Context)*  
<img src="../assets/diagrams/class-diagram-etapa-3-billing-context.svg" alt="Class Diagram - Billing Context" style="width: 100vw;">

### 4.8.1. Database Diagrams

*Figura XX (Database Diagram)*  
<img src="../assets/images/figures/xx-database-diagram.png" alt="Database Diagram" style="width: 100vw;">
