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

Estado: IMPLEMENTADA

Problema

El sistema podía confundir el objetivo del usuario con un medio técnico o una interfaz.

Ejemplo

Usuario:

«Quiero una automatización de reservas para una peluquería.»

El sistema podía desviarse hacia:

«Crear una web para una peluquería.»

Solución

Separar explícitamente:

- objetivo;
- problema;
- sistema;
- medio técnico;
- interfaz;
- mejoras.

La tecnología o interfaz no puede convertirse automáticamente en el objetivo.

Archivo afectado

"01-UNIVERSAL/PROTOCOLO-EJECUCION.md"

Validación

Prueba realizada con el caso de automatización de reservas de una peluquería.

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

Archivo afectado

"01-UNIVERSAL/PROTOCOLO-EJECUCION.md"

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

Inspiración

OpenSpec utiliza una separación explícita entre la fuente de verdad actual y los cambios propuestos.

Archivo afectado

"01-UNIVERSAL/PROTOCOLO-EJECUCION.md"

---

M-004 — Clarificación previa

Estado: PENDIENTE

Objetivo

Resolver ambigüedades antes de diseñar o implementar.

Inspiración

GitHub Spec Kit dispone de una fase específica de "clarify".

Pendiente

Crear mecanismo específico de clarificación dentro del flujo de proyecto.

---

M-005 — Análisis de coherencia

Estado: PENDIENTE

Objetivo

Comprobar que:

objetivo → requisitos → arquitectura → tareas

son coherentes entre sí.

Inspiración

Spec Kit incorpora "analyze" para cruzar los artefactos del proyecto y detectar incoherencias.

---

M-006 — Convergencia

Estado: PENDIENTE

Objetivo

Después de construir, comprobar:

lo especificado ↔ lo implementado

y detectar lo que falta.

Inspiración

Spec Kit incorpora "converge" para evaluar la implementación frente a la especificación.

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

Motivo

Los frameworks analizados resuelven diferentes capas del problema y tienen distintos niveles de ceremonia.

Principio

Reutilizar + adaptar + mejorar.

No:

copiar + depender.

---

M-010 — Especialización en automatización de negocio

Estado: PENDIENTE

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
- servicios externos.

Próxima validación

Automatización de reservas para una peluquería.

---

PRÓXIMAS MEJORAS

M-011

Crear mecanismo formal "CLARIFY".

M-012

Crear mecanismo formal "ANALYZE".

M-013

Crear mecanismo formal "CONVERGE".

M-014

Crear benchmark periódico frente a frameworks externos.

M-015

Definir agentes especializados únicamente cuando la complejidad del proyecto lo justifique.

---

PRINCIPIO DE EVOLUCIÓN

BASE-PROYECTOS debe mejorar mediante:

DETECTAR → DOCUMENTAR → DISEÑAR → IMPLEMENTAR → VALIDAR → REGISTRAR

Nunca mediante cambios silenciosos.

---

REGLA DE MEMORIA

Las decisiones importantes del sistema deben registrarse aquí o en el documento específico que corresponda.

La memoria conversacional puede ayudar a continuar una sesión, pero no constituye la fuente de verdad del sistema.


