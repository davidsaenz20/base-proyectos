# ESTADO DEL PROYECTO

> Estado operativo actual de BASE-PROYECTOS.
>
> Este archivo es la fuente de verdad sobre dónde estamos, qué está terminado, qué está pendiente y cuál es el siguiente trabajo.

---

# 1. ESTADO ACTUAL

**Proyecto:** BASE-PROYECTOS

**Estado:** En desarrollo

**Fase actual:** Fase 1 — Descubrimiento y definición de la BASE

**Objetivo actual:** Consolidar y validar la arquitectura de BASE-PROYECTOS antes de continuar ampliándola.

**Última actualización:** 2026-08-28

---

# 2. ÚLTIMO PUNTO VÁLIDO

Se ha realizado una revisión de la arquitectura general, documentación de control, tipos de proyecto y sistema de trabajo.

Se ha identificado que la estructura general de la BASE está avanzada, pero el sistema de control operativo no estaba reflejando correctamente el estado real del trabajo.

También se ha creado `MODO-TRABAJO.md` en la raíz del repositorio para definir el protocolo de trabajo autónomo entre el usuario y ChatGPT.

---

# 3. TRABAJO COMPLETADO

## Arquitectura general

**Estado:** Avanzado

La estructura principal de BASE-PROYECTOS está definida y organizada por capas.

## Sistema de documentación

**Estado:** Avanzado

Existen estructuras separadas para:

- control;
- documentación universal;
- módulos;
- plantillas;
- tipos de proyecto;
- fixtures;
- proyectos;
- temporal.

## Tipos de proyecto

**Estado:** En desarrollo avanzado

Existe documentación específica para los tipos de proyecto y se ha comprobado la existencia de `APP-MOVIL.md`.

## Modo de trabajo

**Estado:** Definido

Se ha creado:

`MODO-TRABAJO.md`

Su objetivo es permitir trabajo autónomo por bloques y utilizar `.` como comando rápido de continuación.

## Historial

**Estado:** Revisado

Se ha revisado el historial reciente del repositorio para reconstruir el estado del trabajo.

---

# 4. PROBLEMAS IDENTIFICADOS

## Problema 1 — Estado operativo

`00-CONTROL/ESTADO.md` no estaba registrando el estado real del proyecto.

**Consecuencia:** el sistema no podía recuperar de forma fiable el punto exacto de trabajo.

**Acción:** convertir este archivo en la fuente persistente de estado.

---

## Problema 2 — Roadmap incompleto

`00-CONTROL/ROADMAP.md` contiene las fases generales, pero todavía no contiene un roadmap específico del trabajo actual.

**Consecuencia:** define el proceso general, pero no determina con precisión el siguiente trabajo concreto.

**Acción:** completar el roadmap específico después de reconstruir y validar el estado.

---

# 5. TRABAJO PENDIENTE

## Prioridad 1

Auditar completamente la estructura y contenido real de:

`04-TIPOS-PROYECTO/`

Objetivo:

- comprobar todos los tipos existentes;
- comprobar coherencia entre README y archivos;
- detectar tipos faltantes;
- detectar documentación duplicada o contradictoria;
- comprobar que cada tipo contiene lo necesario para el sistema.

---

## Prioridad 2

Auditar `00-CONTROL/`.

Comprobar:

- README;
- ESTADO;
- ROADMAP;
- DECISIONES;
- REGLAS;
- INVENTARIO;
- cualquier documento relacionado.

Objetivo: conseguir un sistema de control coherente y recuperable.

---

## Prioridad 3

Actualizar el roadmap específico.

Debe determinar:

- objetivo actual;
- fases;
- tareas;
- dependencias;
- hitos;
- criterios de finalización.

---

## Prioridad 4

Realizar auditoría global de coherencia.

Comprobar que:

- los documentos se referencian correctamente;
- no existen reglas contradictorias;
- no faltan componentes necesarios;
- no existen archivos obsoletos;
- la estructura responde al objetivo de BASE-PROYECTOS.

---

# 6. SIGUIENTE TAREA

La siguiente tarea lógica es:

**AUDITAR 04-TIPOS-PROYECTO COMPLETAMENTE.**

No realizar cambios estructurales antes de terminar esta auditoría salvo que aparezca un error crítico.

---

# 7. BLOQUEOS

**Bloqueo actual:** Ninguno.

**Intervención del usuario necesaria:** Ninguna después de registrar este estado.

---

# 8. CRITERIO PARA CONTINUAR

Una vez completada la auditoría de `04-TIPOS-PROYECTO`, actualizar este archivo si los resultados modifican:

- fase;
- progreso;
- problemas;
- prioridades;
- siguiente tarea.

---

# 9. PROGRESO ESTIMADO

Estos porcentajes son aproximados y representan progreso real del trabajo, no cantidad de archivos.

| Área | Progreso |
|---|---:|
| Arquitectura | 90% |
| Control | 40% |
| Tipos de proyecto | 70% |
| Documentación | 75% |
| Auditoría global | 20% |
| Validación | 0% |
| Construcción | 0% |
| **TOTAL BASE** | **55%** |

---

# 10. REGLA DE ACTUALIZACIÓN

Este archivo debe actualizarse cuando exista un cambio significativo en:

- estado;
- fase;
- tarea;
- prioridad;
- bloqueo;
- decisión;
- progreso.

No actualizarlo por cada acción trivial.

Su función es permitir recuperar el trabajo incluso si el contexto de la conversación deja de estar disponible.

---

# 11. SIGUIENTE PUNTO DE RECUPERACIÓN

Si se pierde el contexto de la conversación, comenzar desde:

**Fase:** Descubrimiento y definición de BASE

**Área:** `04-TIPOS-PROYECTO`

**Tarea:** Auditoría completa

**Siguiente acción:** revisar README y todos los tipos existentes, contrastarlos entre sí y detectar incoherencias o faltantes.

---

# 12. REGLA FINAL

Este archivo responde:

**¿DÓNDE ESTAMOS?**

**¿QUÉ HEMOS TERMINADO?**

**¿QUÉ ESTÁ PENDIENTE?**

**¿QUÉ ESTÁ BLOQUEADO?**

**¿QUÉ TOCA HACER AHORA?**

El detalle de cómo trabajar pertenece a:

`MODO-TRABAJO.md`

El plan general pertenece a:

`00-CONTROL/ROADMAP.md`
