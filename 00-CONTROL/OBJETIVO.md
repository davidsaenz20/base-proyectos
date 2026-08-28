# OBJETIVO DE BASE-PROYECTOS

## 1. Objetivo principal

Construir una BASE de trabajo reutilizable que permita transformar una idea, necesidad u oportunidad en un proyecto real y funcional.

BASE-PROYECTOS debe proporcionar una metodología estructurada para:

- analizar una necesidad;
- investigar y validar una oportunidad;
- definir requisitos;
- identificar el tipo de proyecto;
- identificar especializaciones;
- seleccionar los módulos necesarios;
- diseñar la arquitectura;
- planificar la ejecución;
- construir la solución;
- probarla;
- validarla;
- desplegarla;
- operarla;
- mejorarla.

El objetivo no es crear documentación por sí misma.

El objetivo es disponer de un sistema que permita **crear proyectos reales de forma reproducible, verificable, eficiente y escalable**.

---

## 2. Problema que resuelve

Cuando se comienza un proyecto desde cero existe riesgo de:

- empezar a construir demasiado pronto;
- olvidar requisitos;
- utilizar herramientas innecesarias;
- elegir una arquitectura inadecuada;
- duplicar trabajo;
- perder decisiones;
- depender de la memoria de una conversación;
- no validar la viabilidad;
- no detectar riesgos;
- no probar correctamente el resultado;
- no disponer de un proceso reproducible.

BASE-PROYECTOS pretende reducir estos problemas proporcionando una estructura común para analizar, diseñar, construir y validar proyectos.

---

## 3. Usuario o destinatario

BASE-PROYECTOS está diseñado para ser utilizado por:

- una persona que desarrolla proyectos;
- un equipo;
- agentes de IA;
- sistemas de automatización;
- procesos híbridos entre personas, IA y automatización.

La BASE debe poder ser comprendida y utilizada sin depender de una conversación concreta.

---

## 4. Resultado esperado

Cuando BASE-PROYECTOS esté suficientemente desarrollado debe permitir iniciar un proyecto nuevo y recorrer un proceso estructurado desde:

```text
IDEA / NECESIDAD
↓
DESCUBRIMIENTO
↓
VIABILIDAD
↓
REQUISITOS
↓
CLASIFICACIÓN
↓
ARQUITECTURA
↓
PLANIFICACIÓN
↓
CONSTRUCCIÓN
↓
INTEGRACIÓN
↓
TESTING
↓
VALIDACIÓN
↓
DESPLIEGUE
↓
OPERACIÓN
↓
MEJORA
```

El sistema debe conservar la trazabilidad entre estas etapas.

---

## 5. Alcance

### Incluido

BASE-PROYECTOS debe cubrir:

- metodología universal;
- principios y reglas;
- análisis previo;
- viabilidad;
- requisitos;
- arquitectura;
- módulos reutilizables;
- tipos de proyecto;
- especializaciones;
- plantillas;
- fixtures;
- testing;
- validación;
- documentación;
- seguridad;
- riesgos;
- despliegue;
- monitorización;
- operación;
- control del proyecto;
- evolución de la propia BASE.

### No incluido

No forma parte del objetivo de la BASE:

- construir automáticamente cualquier proyecto sin supervisión cuando esta sea necesaria;
- sustituir el criterio humano en decisiones que requieran validación humana;
- añadir herramientas o servicios sin una necesidad justificada;
- convertir la documentación en un fin en sí mismo;
- mantener información específica de un proyecto dentro de las capas universales cuando deba pertenecer a un módulo o tipo especializado.

---

## 6. Principios fundamentales

### 6.1 Validar antes de construir

No debe iniciarse una construcción importante sin comprender suficientemente:

- el problema;
- el usuario;
- el objetivo;
- los requisitos;
- las restricciones;
- la viabilidad;
- los riesgos.

### 6.2 Simplicidad

La solución debe ser proporcional al problema.

No deben añadirse componentes innecesarios.

### 6.3 Reutilización

Las soluciones que puedan reutilizarse correctamente deben convertirse en conocimiento, módulos, plantillas o reglas reutilizables.

### 6.4 Trazabilidad

Las decisiones importantes deben poder rastrearse hasta su motivo.

### 6.5 Verificación

La existencia de documentación no demuestra que una metodología funcione.

Los comportamientos importantes deben poder probarse.

### 6.6 Separación de responsabilidades

La información universal debe mantenerse separada de:

- módulos específicos;
- tipos de proyecto;
- especializaciones;
- información exclusiva de un proyecto concreto.

---

## 7. Criterio de éxito

BASE-PROYECTOS se considerará funcional cuando pueda utilizarse para desarrollar un proyecto real siguiendo su metodología y cuando el proceso permita:

- identificar correctamente el problema;
- evaluar la viabilidad;
- definir requisitos;
- clasificar el proyecto;
- seleccionar las estructuras necesarias;
- diseñar una arquitectura coherente;
- ejecutar una construcción;
- realizar pruebas;
- detectar errores;
- validar resultados;
- documentar decisiones;
- desplegar una solución;
- recuperar el estado del proyecto;
- reutilizar la BASE en nuevos proyectos.

El éxito no se medirá por el número de documentos creados.

Se medirá por la **capacidad real del sistema para producir proyectos correctos y funcionales**.

---

## 8. Criterio de calidad

Una solución producida mediante BASE-PROYECTOS debe buscar:

- utilidad real;
- viabilidad económica cuando corresponda;
- simplicidad;
- seguridad;
- mantenibilidad;
- escalabilidad proporcional;
- trazabilidad;
- capacidad de validación;
- documentación suficiente;
- ausencia de complejidad innecesaria.

---

## 9. Evolución

BASE-PROYECTOS no se considera un sistema estático.

Cuando un proyecto real o una prueba demuestre que falta:

- una regla;
- un módulo;
- un tipo;
- una especialización;
- una plantilla;
- una validación;
- un procedimiento;

la BASE podrá evolucionar.

Los cambios importantes deben quedar registrados.

La evolución debe mejorar la capacidad del sistema sin introducir complejidad innecesaria.

---

## 10. Relación con otros documentos

Este archivo define:

**PARA QUÉ EXISTE BASE-PROYECTOS.**

`00-CONTROL/ESTADO.md` define:

**DÓNDE ESTÁ EL PROYECTO ACTUALMENTE.**

`00-CONTROL/ROADMAP.md` define:

**QUÉ TRABAJO DEBE REALIZARSE Y EN QUÉ ORDEN.**

`00-CONTROL/DECISIONES.md` registra:

**QUÉ DECISIONES IMPORTANTES SE HAN TOMADO Y POR QUÉ.**

`MODO-TRABAJO.md` define:

**CÓMO SE EJECUTA EL TRABAJO ENTRE EL USUARIO Y LA IA.**

---

## 11. Restricciones

BASE-PROYECTOS debe evitar:

- documentación duplicada;
- reglas contradictorias;
- estructuras innecesariamente complejas;
- dependencias no justificadas;
- decisiones no documentadas;
- validaciones inexistentes;
- asumir que un archivo está actualizado sin comprobarlo;
- considerar completada una tarea únicamente porque exista documentación sobre ella.

---

## 12. Objetivo final

El objetivo final es disponer de una BASE capaz de actuar como sistema operativo metodológico para la creación de proyectos.

Debe permitir pasar de:

**"Tengo una idea."**

a:

**"Tengo un proyecto analizado, diseñado, construido, probado, validado y funcionando."**

de una forma:

- estructurada;
- reproducible;
- verificable;
- eficiente;
- reutilizable;
- escalable.

---

# ESTADO

**Estado:** Objetivo definido

**Versión:** 2.0

**Última revisión:** 2026-08-28


