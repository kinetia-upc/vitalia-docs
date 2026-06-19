# Recomendaciones

- **Sobre el Roadmap y Siguientes Sprints:** Tras el Avance 2, se recomienda concentrar el siguiente ciclo en completar la cobertura de endpoints faltantes y estabilizar la integración entre frontend y backend. Esto permitirá reemplazar por completo los datos simulados, reducir errores de consumo y validar los flujos principales con información persistente.

- **Validación Temprana y Usabilidad (Testing):** Ahora que se cuenta con una aplicación web funcional y una integración backend en progreso, se recomienda organizar rondas de pruebas de usabilidad con médicos, recepcionistas y administradores. Recolectar feedback sobre navegación, agendamiento, registro clínico y gestión administrativa permitirá realizar ajustes antes de la entrega final.

- **Endpoints Pendientes:** Se recomienda priorizar la implementación y documentación de los endpoints restantes para cerrar brechas funcionales. En el contexto de tenant deben completarse `healthcareCenters`, `branches`, `users` y `appointmentFees`; en el contexto clinical deben completarse `patients`, `doctors`, `specialities` y `doctorSpecialities`.

- **Integraciones de Terceros (APIs):** De cara a la madurez del producto, se recomienda ir analizando la documentación técnica de sistemas de terceros para los módulos secundarios, específicamente la API de RENIEC (para el registro rápido de pacientes y validación de identidad) y las pasarelas de facturación electrónica validadas por SUNAT.

- **Gestión Documental:** Se sugiere mantener el rigor en el flujo de Docs-as-Code, Conventional Commits y evidencias de ejecución. La trazabilidad entre tareas, endpoints, capturas, commits y documentación facilitará la auditoría del proyecto y permitirá demostrar con mayor claridad el avance técnico alcanzado.
