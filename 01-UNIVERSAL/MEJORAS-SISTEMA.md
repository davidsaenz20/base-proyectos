MEJORAS DEL SISTEMA

Propósito

Registrar de forma persistente las mejoras, decisiones y aprendizajes que modifican o perfeccionan BASE-PROYECTOS.

Este archivo evita que las decisiones importantes dependan de la memoria de una conversación.

---

ESTADO

Sistema: BASE-PROYECTOS
Estado: En evolución
Objetivo: Convertir BASE-PROYECTOS en un sistema capaz de guiar proyectos reales de automatización desde la idea hasta un sistema validado y funcionando.

---

REGLAS DE ESTE REGISTRO

Cada mejora debe contener:

- identificador;
- fecha;
- origen;
- problema detectado;
- solución;
- archivos afectados;
- estado;
- validación.

Una mejora no se considera incorporada hasta que los archivos afectados hayan sido actualizados y la modificación haya sido validada.

---

MEJORAS

M-001 — Bloqueo del objetivo primario

Estado: IMPLEMENTADA Y VALIDADA

Problema

El sistema podía confundir el objetivo del usuario con un medio técnico o una interfaz.

Solución

Separar explícitamente:

- objetivo;
- problema;
- sistema;
- medio técnico;
- interfaz;
- mejoras.

La tecnología o interfaz no puede convertirse automáticamente en el objetivo.

Validación

Prueba realizada con el caso de automatización de reservas para una peluquería.

Resultado: correcto.

---

M-002 — Contexto mínimo suficiente

Estado: IMPLEMENTADA

Problema

Cargar demasiada documentación puede introducir contradicciones y consumir contexto innecesariamente.

Solución

Utilizar únicamente el contexto necesario para el paso actual.

Objetivo

Mantener:

- foco;
- continuidad;
- coherencia;
- eficiencia.

---

M-003 — Separación entre realidad y propuesta

Estado: IMPLEMENTADA

Problema

Una propuesta futura puede confundirse con una funcionalidad ya existente.

Solución

Distinguir:

- estado actual;
- propuesta;
- implementación;
- evidencia.

Principio

Nunca presentar una propuesta como si ya estuviera implementada.

---

M-004 — Clarificación previa

Estado: IMPLEMENTADA Y VALIDADA

Objetivo

Resolver ambigüedades antes de diseñar o implementar.

Mecanismo

Durante CLARIFY, la IA debe:

1. identificar el objetivo primario;
2. detectar ambigüedades;
3. identificar información desconocida;
4. determinar qué cuestiones pueden cambiar sustancialmente el proyecto;
5. preguntar al usuario cuando sea necesario;
6. continuar únicamente con una interpretación suficientemente clara.

Validación

Probado durante la prueba de automatización de una solución para propietarios que desean alquilar una vivienda.

---

M-005 — Análisis de coherencia

Estado: IMPLEMENTADA Y VALIDADA

Objetivo

Comprobar que:

objetivo → requisitos → arquitectura → tareas → implementación

son coherentes entre sí.

Mecanismo

Durante ANALYZE se deben detectar:

- contradicciones;
- requisitos faltantes;
- desviaciones;
- decisiones no justificadas;
- información crítica desconocida;
- diferencias entre lo planificado y lo realizado.

Validación

Durante la prueba se detectó que el objetivo de crear una solución para propietarios no debía convertirse automáticamente en una simple web.

Resultado: correcto.

---

M-006 — Convergencia

Estado: IMPLEMENTADA Y VALIDADA

Objetivo

Después de construir, comprobar:

lo especificado ↔ lo implementado

y detectar lo que falta.

Mecanismo

CONVERGE debe comprobar:

- requisitos cumplidos;
- requisitos pendientes;
- funcionalidades implementadas;
- funcionalidades no implementadas;
- pruebas realizadas;
- evidencias disponibles;
- desviaciones existentes.

Validación

Validado conceptualmente durante las pruebas del sistema.

---

M-007 — Complejidad adaptativa

Estado: IMPLEMENTADA

Objetivo

Evitar aplicar la misma cantidad de documentación y controles a todos los proyectos.

Principio

Proyecto pequeño:

menos ceremonia.

Proyecto complejo:

más controles, documentación y validaciones.

---

M-008 — Trazabilidad completa

Estado: IMPLEMENTADA

Flujo

OBJETIVO

↓

REQUISITO

↓

DECISIÓN

↓

ARQUITECTURA

↓

TAREA

↓

IMPLEMENTACIÓN

↓

PRUEBA

↓

EVIDENCIA

Cada elemento importante debe poder relacionarse con el anterior y el siguiente cuando corresponda.

---

M-009 — Estrategia de evolución

Estado: IMPLEMENTADA

Decisión

No copiar íntegramente ningún framework externo.

BASE-PROYECTOS permanece como núcleo.

Se incorporarán selectivamente mecanismos útiles de:

- GitHub Spec Kit;
- OpenSpec;
- BMAD;
- GSD;
- otros sistemas relevantes.

Principio

Reutilizar + adaptar + mejorar.

No:

copiar + depender.

---

M-010 — Especialización en automatización de negocio

Estado: IMPLEMENTADA Y VALIDADA CONCEPTUALMENTE

Objetivo

Orientar BASE-PROYECTOS específicamente hacia:

IDEA → AUTOMATIZACIÓN → INTEGRACIONES → PRUEBAS → PRODUCCIÓN → MANTENIMIENTO

y no limitarlo al desarrollo de software tradicional.

Ejemplos

- n8n;
- WhatsApp;
- APIs;
- calendarios;
- bases de datos;
- CRM;
- formularios;
- automatizaciones;
- agentes IA;
- servicios externos;
- generación automática de contenidos;
- generación y mantenimiento de sitios web.

Validación

La prueba de reservas de peluquería y la nueva prueba de solución automatizada para propietarios demuestran que el sistema puede trabajar con proyectos donde la automatización es el objetivo principal.

---

M-011 — Gestión de aportaciones del usuario durante el proyecto

Estado: INCORPORADA AL PROTOCOLO

Origen

Prueba de creación de una solución especializada para propietarios que desean alquilar una vivienda.

Problema

El usuario puede aportar nuevas ideas después de haber definido inicialmente el proyecto.

Ejemplo:

Objetivo inicial:

Crear una solución para ayudar a propietarios que quieren alquilar una vivienda.

Nueva aportación:

Ayudar también con documentación, papeleo y trámites.

La nueva aportación no debe:

- perderse;
- convertirse automáticamente en requisito;
- modificar silenciosamente el objetivo;
- interrumpir innecesariamente el trabajo actual.

Solución

Toda nueva aportación debe pasar por:

APORTACIÓN

↓

CLASIFICACIÓN

↓

ANÁLISIS

↓

DECISIÓN

↓

REGISTRO

↓

INCORPORACIÓN AL ALCANCE O BACKLOG

Clasificación mínima

La aportación puede ser:

- información adicional;
- requisito;
- ampliación;
- mejora;
- idea futura;
- cambio de alcance;
- cambio del objetivo;
- bloqueo;
- decisión del usuario.

Regla

Una aportación del usuario tiene prioridad sobre una suposición de la IA, pero no debe incorporarse automáticamente al alcance si cambia significativamente el proyecto.

Si modifica el objetivo primario, requiere confirmación y registro explícito.

Validación

Detectada durante la prueba actual.

Resultado: mecanismo necesario y aprobado para incorporación al sistema.

---

M-012 — Progreso objetivo basado en trabajo real

Estado: INCORPORADA AL PROTOCOLO

Origen

Prueba real de ejecución mediante órdenes repetidas de:

«Sigue trabajando».

Problema

La IA estaba comunicando porcentajes como:

20% → 30% → 40% → 50%

sin que dichos porcentajes procedieran necesariamente de tareas reales completadas.

Esto puede crear una falsa percepción del estado del proyecto.

Solución

El porcentaje de ejecución debe calcularse a partir del trabajo real registrado en el roadmap o sistema de estado.

Nunca debe utilizarse un porcentaje subjetivo simplemente para comunicar sensación de progreso.

Principio

PROGRESO = trabajo completado / trabajo planificado

Cuando las tareas tengan diferente peso, puede utilizarse un cálculo ponderado.

Regla

La IA debe distinguir:

- progreso del proyecto;
- progreso de la fase;
- progreso del paso;
- trabajo realizado durante la sesión.

Si no existe información suficiente para calcular un porcentaje fiable:

no inventar el porcentaje.

Debe comunicarse:

«progreso no calculable todavía»

o utilizarse únicamente un estado cualitativo.

Validación

Problema detectado durante la prueba actual.

Resultado: mejora confirmada como necesaria.

---

PRÓXIMAS MEJORAS

M-013 — Benchmark periódico frente a sistemas externos

Comparar periódicamente BASE-PROYECTOS con sistemas relevantes para incorporar mecanismos útiles sin copiar metodologías completas.

---

M-014 — Agentes especializados adaptativos

Definir agentes especializados únicamente cuando la complejidad del proyecto lo justifique.

---

M-015 — Métricas objetivas de proyecto

Definir métricas adicionales para medir:

- cumplimiento;
- calidad;
- cobertura;
- errores;
- validaciones;
- tiempo;
- deuda;
- riesgo.

---

PRINCIPIO DE EVOLUCIÓN

BASE-PROYECTOS debe mejorar mediante:

DETECTAR → DOCUMENTAR → DISEÑAR → IMPLEMENTAR → VALIDAR → REGISTRAR

Nunca mediante cambios silenciosos.

---

REGLA DE MEMORIA

Las decisiones importantes del sistema deben registrarse aquí o en el documento específico que corresponda.

La memoria conversacional puede ayudar a continuar una sesión, pero no constituye la fuente de verdad del sistema.

---

PRINCIPIO DE APORTACIONES

El usuario puede introducir nuevas ideas, requisitos, cambios o información en cualquier momento durante la ejecución.

El sistema debe poder incorporarlos sin perder:

- objetivo;
- contexto;
- trazabilidad;
- decisiones anteriores;
- trabajo ya validado.

Una nueva aportación no implica automáticamente rehacer el proyecto.

Debe analizarse primero.

---

PRINCIPIO DE PROGRESO

El sistema no debe utilizar porcentajes subjetivos para aparentar avance.

Todo porcentaje debe poder explicarse mediante:

ROADMAP + TAREAS + ESTADO + EVIDENCIA

Si no puede justificarse:

no se comunica como porcentaje objetivo.

---

PRINCIPIO FINAL

BASE-PROYECTOS debe ser capaz de transformar:

IDEA DEL USUARIO

+ 

APORTACIONES DEL USUARIO

↓

CLARIFY

↓

ANALYZE

↓

PLANIFICACIÓN

↓

EJECUCIÓN

↓

VALIDACIÓN

↓

CONVERGE

↓

SISTEMA FUNCIONANDO EN LA REALIDAD

manteniendo siempre al usuario como autoridad sobre el objetivo y utilizando la IA como sistema de análisis, ejecución y asistencia.


