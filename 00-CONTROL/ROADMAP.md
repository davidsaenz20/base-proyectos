# ROADMAP DEL PROYECTO

> Plan específico de ejecución de BASE-PROYECTOS.
>
> Define qué trabajo debe realizarse, en qué orden, qué entregables deben producirse y qué condiciones permiten avanzar.
>
> El estado operativo actual se registra exclusivamente en `00-CONTROL/ESTADO.md`.

---

# 1. OBJETIVO DEL ROADMAP

**Resultado que debe conseguir BASE-PROYECTOS:**

Construir una BASE de trabajo reutilizable que permita transformar una idea o necesidad en un proyecto real, desde el descubrimiento inicial hasta su construcción, validación, despliegue y operación.

La BASE debe permitir:

- analizar correctamente una necesidad;
- identificar el tipo de proyecto;
- seleccionar los módulos necesarios;
- definir requisitos;
- diseñar una arquitectura;
- planificar la construcción;
- ejecutar el proyecto;
- validar el resultado;
- detectar errores;
- documentar decisiones;
- reutilizar conocimientos y estructuras;
- trabajar de forma reproducible;
- evitar construir soluciones innecesariamente complejas;
- mantener trazabilidad entre necesidad, diseño, construcción y validación.

El objetivo final no es crear documentación por sí misma.

El objetivo es disponer de un sistema de trabajo que pueda utilizarse para crear proyectos reales y funcionales.

---

# 2. PRINCIPIOS DE EJECUCIÓN

## 2.1 Validar antes de construir

No debe comenzar una construcción importante mientras no exista suficiente información para determinar:

- qué problema se resuelve;
- para quién;
- qué resultado se espera;
- qué requisitos existen;
- qué restricciones existen;
- qué arquitectura es necesaria.

---

## 2.2 Simplicidad proporcional

La solución debe ser tan sencilla como sea posible sin comprometer los requisitos.

No deben añadirse:

- herramientas;
- servicios;
- APIs;
- bases de datos;
- automatizaciones;
- infraestructura;
- módulos;

si no existe una necesidad justificada.

---

## 2.3 Evidencia antes que suposición

Cuando sea posible comprobar algo, debe comprobarse.

No debe considerarse:

- creado;
- actualizado;
- disponible;
- funcional;
- validado;

simplemente porque exista una afirmación de que lo está.

---

## 2.4 Validación progresiva

Cada etapa importante debe validarse antes de construir encima de ella.

La estrategia recomendada es:

ANALIZAR
↓
DEFINIR
↓
VALIDAR
↓
CONSTRUIR
↓
PROBAR
↓
VALIDAR
↓
ESCALAR

---

## 2.5 Reutilización

Cuando una solución, regla, módulo o estructura pueda reutilizarse correctamente, debe incorporarse a la BASE.

No duplicar conocimiento innecesariamente.

---

# 3. FASES DE EJECUCIÓN

## FASE 1 — DESCUBRIMIENTO Y DEFINICIÓN

**Objetivo:**

Comprender el problema, usuario, contexto, oportunidad y alcance.

**Trabajo:**

- investigar;
- definir el problema;
- identificar usuario/cliente;
- definir objetivo;
- determinar alcance;
- formular hipótesis;
- evaluar viabilidad inicial;
- identificar restricciones;
- identificar riesgos iniciales.

**Entregable:**

Definición validada del proyecto.

**Criterio de finalización:**

- problema definido;
- objetivo definido;
- usuario identificado;
- alcance establecido;
- hipótesis relevantes identificadas;
- viabilidad inicial evaluada;
- riesgos principales identificados.

---

## FASE 2 — REQUISITOS

**Objetivo:**

Convertir la idea en requisitos verificables.

**Trabajo:**

- requisitos funcionales;
- requisitos técnicos;
- restricciones;
- requisitos de seguridad;
- requisitos legales cuando correspondan;
- requisitos de rendimiento cuando correspondan;
- criterios de aceptación.

**Entregable:**

Requisitos documentados y verificables.

**Criterio de finalización:**

Todos los requisitos críticos están definidos y pueden comprobarse.

---

## FASE 3 — TIPO Y CLASIFICACIÓN DEL PROYECTO

**Objetivo:**

Determinar qué tipo de proyecto se está construyendo.

**Trabajo:**

- identificar tipo principal;
- identificar especializaciones;
- identificar comportamiento específico;
- identificar módulos derivados;
- comprobar fixtures aplicables;
- identificar necesidades particulares.

**Entregable:**

Clasificación del proyecto.

**Criterio de finalización:**

El tipo y las especializaciones relevantes están identificados y existe cobertura de prueba suficiente.

---

## FASE 4 — DISEÑO Y ARQUITECTURA

**Objetivo:**

Definir cómo se construirá la solución.

**Trabajo:**

- arquitectura;
- componentes;
- datos;
- integraciones;
- APIs;
- seguridad;
- almacenamiento;
- interfaces;
- decisiones técnicas;
- dependencias.

**Entregable:**

Arquitectura validada.

**Criterio de finalización:**

La solución es técnicamente viable, proporcional y construible.

---

## FASE 5 — PLANIFICACIÓN TÉCNICA

**Objetivo:**

Convertir la arquitectura en un plan ejecutable.

**Trabajo:**

- dividir trabajo;
- definir tareas;
- establecer dependencias;
- establecer orden;
- determinar herramientas;
- determinar entorno;
- establecer criterios de validación por bloque.

**Entregable:**

Plan técnico de construcción.

**Criterio de finalización:**

Existe una secuencia clara y ejecutable.

---

## FASE 6 — PREPARACIÓN DEL ENTORNO

**Objetivo:**

Disponer de los recursos necesarios.

**Trabajo:**

- cuentas;
- servicios;
- repositorios;
- credenciales;
- variables;
- herramientas;
- dominios;
- hosting;
- APIs;
- entornos de prueba.

**Entregable:**

Entorno preparado.

**Criterio de finalización:**

El entorno permite iniciar la construcción sin bloqueos conocidos.

---

## FASE 7 — CONSTRUCCIÓN

**Objetivo:**

Implementar la solución.

**Trabajo:**

- componentes;
- interfaces;
- automatizaciones;
- integraciones;
- lógica;
- almacenamiento;
- workflows;
- APIs;
- documentación necesaria.

**Entregable:**

Primera implementación funcional.

**Criterio de finalización:**

Las funcionalidades previstas para el bloque están implementadas y pueden probarse.

---

## FASE 8 — INTEGRACIÓN

**Objetivo:**

Conectar los componentes y comprobar el flujo conjunto.

**Trabajo:**

- APIs;
- servicios externos;
- flujo de datos;
- automatizaciones;
- manejo de errores;
- recuperación.

**Entregable:**

Sistema integrado.

**Criterio de finalización:**

El flujo previsto puede recorrer correctamente todos los componentes necesarios.

---

## FASE 9 — TESTING TÉCNICO

**Objetivo:**

Detectar y corregir errores técnicos.

**Trabajo:**

- pruebas funcionales;
- pruebas de integración;
- pruebas negativas;
- pruebas de errores;
- seguridad;
- rendimiento;
- regresión.

**Entregable:**

Resultados de testing y correcciones.

**Criterio de finalización:**

No existen errores críticos conocidos que impidan pasar a validación.

---

## FASE 10 — VALIDACIÓN

**Objetivo:**

Comprobar que la solución cumple los requisitos.

**Trabajo:**

- criterios de aceptación;
- pruebas funcionales;
- pruebas de usuario;
- evidencias;
- comparación con requisitos;
- documentación de incidencias.

**Entregable:**

Validación documentada.

**Criterio de finalización:**

Los criterios de aceptación están cumplidos o las excepciones están documentadas y aceptadas.

---

## FASE 11 — DESPLIEGUE

**Objetivo:**

Poner la solución en el entorno real.

**Trabajo:**

- configuración;
- publicación;
- dominio;
- servicios;
- seguridad;
- backups;
- comprobaciones post-despliegue.

**Entregable:**

Sistema desplegado.

**Criterio de finalización:**

El sistema está disponible en el entorno objetivo y supera las comprobaciones iniciales.

---

## FASE 12 — PRUEBA REAL DE EXTREMO A EXTREMO

**Objetivo:**

Comprobar el flujo completo en condiciones reales o representativas.

**Trabajo:**

- entrada real;
- procesamiento real;
- integraciones reales;
- salida real;
- errores;
- recuperación;
- intervención manual.

**Entregable:**

Evidencia de funcionamiento extremo a extremo.

**Criterio de finalización:**

El flujo completo funciona sin intervención manual no prevista.

---

## FASE 13 — MONITORIZACIÓN

**Objetivo:**

Asegurar que el sistema puede supervisarse.

**Trabajo:**

- métricas;
- logs;
- alertas;
- disponibilidad;
- errores;
- consumo;
- recuperación.

**Entregable:**

Sistema de monitorización.

**Criterio de finalización:**

Los fallos relevantes pueden detectarse y gestionarse.

---

## FASE 14 — OPERACIÓN

**Objetivo:**

Definir cómo se utilizará y mantendrá el sistema.

**Trabajo:**

- procedimientos;
- mantenimiento;
- soporte;
- incidencias;
- backups;
- responsabilidades;
- actualización;
- documentación operativa.

**Entregable:**

Procedimiento operativo.

**Criterio de finalización:**

Existe un procedimiento reproducible de operación y mantenimiento.

---

## FASE 15 — OPTIMIZACIÓN

**Objetivo:**

Mejorar el sistema después de comprobar su funcionamiento.

**Trabajo:**

- rendimiento;
- costes;
- fiabilidad;
- automatización;
- UX;
- escalabilidad;
- mejoras basadas en datos reales.

**Entregable:**

Mejoras validadas.

**Criterio de finalización:**

Cada mejora aporta un beneficio verificable.

---

## FASE 16 — CIERRE

**Objetivo:**

Consolidar el proyecto y dejarlo documentado y reproducible.

**Trabajo:**

- documentación final;
- evidencias;
- decisiones;
- lecciones aprendidas;
- configuración final;
- criterios de cierre;
- conocimientos reutilizables.

**Entregable:**

Proyecto cerrado y reproducible.

**Criterio de finalización:**

Otra persona puede comprender, operar y mantener el sistema con la documentación disponible.

---

# 4. DEPENDENCIAS PRINCIPALES

Las dependencias deben determinarse durante el avance del proyecto.

Categorías principales:

- información;
- usuarios;
- datos;
- APIs;
- servicios externos;
- cuentas;
- credenciales;
- hosting;
- dominio;
- infraestructura;
- herramientas;
- módulos;
- requisitos legales;
- recursos humanos.

Una dependencia no debe considerarse disponible hasta que haya sido comprobada.

---

# 5. HITOS

## HITO 1 — BASE ESTRUCTURADA

**Resultado:**

La estructura fundamental de BASE-PROYECTOS está definida.

**Criterio:**

Las capas principales existen y tienen responsabilidades claras.

---

## HITO 2 — TIPOS DE PROYECTO DEFINIDOS

**Resultado:**

Los tipos de proyecto principales y sus especializaciones relevantes están documentados.

**Criterio:**

Cada especialización con comportamiento propio dispone de cobertura adecuada.

---

## HITO 3 — SISTEMA DE PRUEBAS

**Resultado:**

Los fixtures y el protocolo de pruebas permiten validar comportamientos.

**Criterio:**

Existen pruebas positivas y negativas y criterios PASS/FAIL claros.

---

## HITO 4 — CONTROL OPERATIVO

**Resultado:**

El sistema de control permite recuperar el estado real del proyecto.

**Criterio:**

`ESTADO.md`, `ROADMAP.md` y documentos de control son coherentes entre sí.

---

## HITO 5 — PRIMER PROYECTO REAL

**Resultado:**

BASE-PROYECTOS se utiliza para desarrollar un proyecto real.

**Criterio:**

El proyecto puede recorrer el proceso desde la entrada hasta la validación.

---

## HITO 6 — VALIDACIÓN END-TO-END

**Resultado:**

Un proyecto real creado mediante la BASE funciona en condiciones reales.

**Criterio:**

El flujo completo funciona y existe evidencia.

---

## HITO 7 — BASE REUTILIZABLE

**Resultado:**

BASE-PROYECTOS puede utilizarse para nuevos proyectos sin rehacer su estructura fundamental.

**Criterio:**

Un nuevo proyecto puede comenzar utilizando la BASE existente.

---

# 6. CRITERIOS DE AVANCE ENTRE FASES

No se debe avanzar únicamente porque una fase haya consumido tiempo.

Para avanzar debe cumplirse su criterio de finalización.

Si falta información crítica:

**REQUIERE VALIDACIÓN**

Si existe un error que impide continuar:

**BLOQUEADO**

Si la fase cumple sus criterios:

**COMPLETADA**

Si aún no se ha ejecutado:

**PENDIENTE**

---

# 7. GESTIÓN DE CAMBIOS DEL PLAN

Cuando una auditoría o una prueba demuestre que el plan debe cambiar:

**Fecha:**

**Cambio:**

**Motivo:**

**Impacto:**

**Nueva prioridad:**

**Dependencias afectadas:**

Los cambios importantes deben reflejarse también en `ESTADO.md` cuando afecten al estado operativo.

---

# 8. REGLAS DE PRIORIZACIÓN

Cuando existan varias tareas posibles, priorizar:

1. bloqueos;
2. errores críticos;
3. inconsistencias de arquitectura;
4. problemas de control;
5. requisitos faltantes;
6. validaciones;
7. construcción;
8. mejoras;
9. optimización.

No optimizar una parte que todavía no ha sido validada.

---

# 9. RELACIÓN CON OTROS DOCUMENTOS

Este documento define:

**QUÉ TRABAJO HAY QUE REALIZAR.**

**EN QUÉ ORDEN.**

**QUÉ ENTREGABLE PRODUCE CADA FASE.**

**QUÉ CRITERIO PERMITE CONSIDERARLA TERMINADA.**

---

`00-CONTROL/ESTADO.md` define:

**DÓNDE ESTAMOS AHORA.**

**QUÉ ESTÁ TERMINADO.**

**QUÉ ESTÁ PENDIENTE.**

**QUÉ ESTÁ BLOQUEADO.**

**QUÉ TOCA HACER AHORA.**

---

`MODO-TRABAJO.md` define:

**CÓMO DEBE EJECUTARSE EL TRABAJO ENTRE EL USUARIO Y LA IA.**

---

`05-FIXTURES/PROTOCOLO-PRUEBAS.md` define:

**CÓMO DEBEN VALIDARSE LOS FIXTURES.**

---

# 10. REGLA FINAL

El roadmap no debe convertirse en una lista estática de tareas.

Debe servir como estructura de planificación.

Cuando el trabajo real demuestre que una tarea, dependencia o fase debe cambiar, el roadmap puede modificarse.

Toda modificación importante debe conservar la trazabilidad del motivo.

El objetivo del roadmap es conseguir que BASE-PROYECTOS pase de:

IDEA
↓
ANÁLISIS
↓
DEFINICIÓN
↓
DISEÑO
↓
CONSTRUCCIÓN
↓
VALIDACIÓN
↓
DESPLIEGUE
↓
OPERACIÓN
↓
MEJORA

de forma reproducible, verificable y proporcional.

---

# ESTADO

**Estado:** Roadmap estructurado y pendiente de ejecución progresiva.

**Versión:** 2.0

**Última revisión:** 2026-08-28


