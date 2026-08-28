# DECISIONES DEL PROYECTO

Este archivo registra las decisiones importantes tomadas durante el desarrollo de BASE-PROYECTOS.

## REGLA

Las decisiones deben quedar registradas para evitar depender de la memoria de la conversación.

No se deben borrar decisiones anteriores.

Si una decisión cambia, se registra una nueva entrada indicando qué ha cambiado y por qué.

---

## Decisión 001

**Fecha:** 2026-08-27

**Tema:** Separación de afiliación respecto a la capa universal

**Decisión:**

El conocimiento específico de proyectos de afiliación automatizada debe residir en `02-MODULOS/MODULO-AFILIACION-AUTOMATIZADA.md` y no dentro de `01-UNIVERSAL`.

La especialización correspondiente a webs de afiliación reside en `04-TIPOS-PROYECTO/WEB-AFILIACION.md`.

**Motivo:**

La capa universal debe contener reglas aplicables a cualquier proyecto.

El conocimiento específico de afiliación debe ser reutilizable mediante un módulo y, cuando corresponda, mediante un tipo de proyecto especializado.

**Impacto:**

Se evita mezclar conocimiento específico de un modelo de negocio con las reglas universales.

**Estado:** Vigente

---

## Decisión 002

**Fecha:** 2026-08-27

**Tema:** Incorporación del tipo APP MÓVIL

**Decisión:**

Se incorpora `04-TIPOS-PROYECTO/APP-MOVIL.md` como definición específica para proyectos de aplicaciones móviles.

**Motivo:**

La BASE debe poder trabajar con aplicaciones móviles sin depender únicamente de reglas genéricas.

**Impacto:**

Los proyectos móviles disponen de una metodología específica dentro de la capa de tipos de proyecto.

**Estado:** Vigente

---

## Decisión 003

**Fecha:** 2026-08-27

**Tema:** Fixtures verificables

**Decisión:**

Los fixtures de `05-FIXTURES` deben poder utilizarse como pruebas verificables y no limitarse a ser ejemplos descriptivos.

Se establece `05-FIXTURES/PROTOCOLO-PRUEBAS.md` como referencia para definir estas pruebas.

**Motivo:**

La existencia de documentación no demuestra que la metodología funcione.

Los fixtures deben permitir comprobar entradas, procesos, resultados y criterios PASS/FAIL.

**Impacto:**

BASE-PROYECTOS puede validarse mediante casos controlados antes de utilizarse en proyectos reales.

**Estado:** Vigente

---

## Decisión 004

**Fecha:** 2026-08-27

**Tema:** Inventario documental

**Decisión:**

`00-CONTROL/INVENTARIO-DOCUMENTOS.md` será el registro de referencia de la estructura documental real de BASE-PROYECTOS.

Debe mantenerse sincronizado con el árbol real del repositorio.

**Motivo:**

La arquitectura documental debe poder auditarse sin depender de la memoria de la conversación.

**Impacto:**

Los nuevos documentos y cambios estructurales deben reflejarse en el inventario.

**Estado:** Vigente

---

## Decisión 005

**Fecha:** 2026-08-28

**Tema:** Auditoría cruzada de capas

**Decisión:**

Antes de iniciar un proyecto real se realizará una auditoría cruzada entre las capas de control, universal, módulos, plantillas, tipos de proyecto, fixtures y proyectos.

**Motivo:**

No basta con comprobar cada documento individualmente.

También debe comprobarse que las capas son compatibles entre sí y que no existen contradicciones, duplicidades o referencias a documentos inexistentes.

**Impacto:**

La validación de BASE-PROYECTOS pasa a considerar tanto la integridad individual de los documentos como la coherencia entre capas.

**Estado:** Vigente

---

## ESTADO

**Última decisión registrada:** 005

**Estado del registro:** Activo

**Última actualización:** 2026-08-28

