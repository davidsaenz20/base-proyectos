BENCHMARK DEL SISTEMA

Propósito

Comparar BASE-PROYECTOS con sistemas y metodologías externas relevantes para identificar:

- capacidades que ya tenemos;
- carencias;
- mecanismos reutilizables;
- diferencias;
- posibles ventajas;
- decisiones de evolución.

Este documento no pretende demostrar que BASE-PROYECTOS sea superior.

Su función es mejorarlo con evidencia.

---

SISTEMAS ANALIZADOS

GitHub Spec Kit

Fortalezas

- flujo estructurado;
- especificación antes de implementación;
- clarificación;
- análisis de coherencia;
- convergencia entre especificación e implementación;
- planificación y tareas.

Elementos interesantes para BASE-PROYECTOS

ADOPTAR / ADAPTAR

- CLARIFY;
- ANALYZE;
- CONVERGE.

Fuente

GitHub Spec Kit.

---

OpenSpec

Fortalezas

- separación entre estado actual y cambios propuestos;
- propuestas auditables;
- especificaciones;
- tareas;
- archivo de cambios;
- validación;
- archivado de cambios.

Elementos interesantes para BASE-PROYECTOS

ADOPTAR / ADAPTAR

- separación fuente de verdad / propuesta;
- cambios auditables;
- requisitos con escenarios;
- archivo histórico de cambios.

Fuente

Fission-AI OpenSpec.

---

BMAD

Fortalezas

- metodología completa;
- fases;
- agentes especializados;
- producto;
- arquitectura;
- desarrollo;
- testing;
- gates.

Elementos interesantes

ADOPTAR SELECTIVAMENTE

- especialización por rol;
- gates de fase;
- profundidad adaptativa.

Riesgo

Demasiada ceremonia para proyectos pequeños.

Fuente

Comparativa de frameworks 2026.

---

GSD

Fortalezas

- ingeniería de contexto;
- planificación;
- ejecución por etapas;
- verificación;
- persistencia de estado;
- control del deterioro del contexto.

Elementos interesantes

ADOPTAR SELECTIVAMENTE

- contexto mínimo suficiente;
- recuperación estructurada;
- verificación;
- gates.

Riesgo

Puede introducir demasiada estructura en automatizaciones sencillas.

Fuente

Comparativa de frameworks 2026.

---

COMPARACIÓN

Capacidad| BASE-PROYECTOS| Spec Kit| OpenSpec| BMAD| GSD
Objetivo| 🟢| 🟢| 🟢| 🟢| 🟢
Especificación| 🟡| 🟢| 🟢| 🟢| 🟢
Clarificación| 🟡| 🟢| 🟡| 🟢| 🟢
Análisis coherencia| 🟡| 🟢| 🟡| 🟢| 🟢
Convergencia| 🟡| 🟢| 🟡| 🟢| 🟢
Cambios auditables| 🟢| 🟡| 🟢| 🟢| 🟢
Estado persistente| 🟢| 🟡| 🟢| 🟢| 🟢
Context engineering| 🟢| 🟡| 🟢| 🟢| 🟢
Agentes especializados| 🟡| 🟡| 🟡| 🟢| 🟢
Adaptación de complejidad| 🟢| 🟡| 🟢| 🟢| 🟢
Automatización de negocio| 🟢| 🟡| 🟡| 🟡| 🟡
n8n / APIs / integraciones| 🟢| 🟡| 🟡| 🟡| 🟡
Producción| 🟢| 🟡| 🟡| 🟢| 🟢

Nota: esta tabla es una evaluación interna de BASE-PROYECTOS y no una puntuación oficial de los frameworks.

---

ESTRATEGIA

No adoptar un framework externo completo.

Adoptar mecanismos concretos cuando aporten valor.

Prioridad 1

CLARIFY

Prioridad 2

ANALYZE

Prioridad 3

CONVERGE

Prioridad 4

Cambios auditables.

Prioridad 5

Agentes especializados.

Prioridad 6

Contexto adaptativo.

---

HIPÓTESIS DIFERENCIAL

BASE-PROYECTOS pretende especializarse en:

PROYECTOS DE AUTOMATIZACIÓN DE NEGOCIO

en lugar de limitarse a:

DESARROLLO DE SOFTWARE CON IA

La hipótesis debe validarse mediante proyectos reales.

---

PRÓXIMA PRUEBA

Proyecto:

Automatización de reservas para una peluquería.

Objetivo:

Comprobar si BASE-PROYECTOS puede llevar un proyecto de automatización desde:

IDEA

hasta:

SISTEMA FUNCIONANDO

sin perder:

- objetivo;
- requisitos;
- contexto;
- trazabilidad;
- validación.

---

REGLA DEL BENCHMARK

Cada nueva comparación debe responder:

1. ¿Qué hace mejor el sistema externo?
2. ¿Lo necesitamos?
3. ¿Podemos implementarlo nosotros?
4. ¿Qué archivo afecta?
5. ¿Cómo lo validamos?
6. ¿Mejora realmente el resultado?

No se incorporará una función únicamente porque otro framework la tenga.


