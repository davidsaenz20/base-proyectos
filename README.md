# BASE-PROYECTOS

Sistema maestro para diseñar, validar, construir, automatizar y desplegar proyectos digitales.

## Objetivo

Convertir una idea de negocio o proyecto en un sistema ejecutable, siguiendo una metodología estructurada y reutilizable.

El sistema debe permitir avanzar desde:

**IDEA → VIABILIDAD → DISEÑO → CONSTRUCCIÓN → PRUEBAS → PUBLICACIÓN → VALIDACIÓN → MEJORA**

## Arquitectura

El repositorio se organiza por capas:

- `00-CONTROL/` — control, estado, decisiones, roadmap e inventario.
- `01-UNIVERSAL/` — reglas y metodología común a todos los proyectos.
- `02-MODULOS/` — capacidades técnicas reutilizables.
- `03-PLANTILLAS/` — estructuras y componentes reutilizables.
- `04-TIPOS-PROYECTO/` — metodologías específicas según el tipo de proyecto.
- `05-FIXTURES/` — pruebas reproducibles de los distintos tipos de proyecto.
- `06-PROYECTOS/` — proyectos reales.
- `temporal/` — documentación provisional de trabajo.

## Cómo funciona

BASE-PROYECTOS no debe limitarse a documentar ideas.

Su finalidad es servir como sistema operativo de trabajo para que ChatGPT pueda:

1. analizar una idea;
2. estudiar su viabilidad;
3. definir requisitos;
4. diseñar la arquitectura;
5. seleccionar módulos y plantillas;
6. construir el proyecto cuando las herramientas disponibles lo permitan;
7. ejecutar y documentar pruebas;
8. detectar errores o bloqueos;
9. indicar exactamente qué intervención manual necesita el usuario;
10. continuar desde el punto correcto después de cada intervención;
11. validar el resultado;
12. preparar la publicación y puesta en funcionamiento;
13. medir el resultado;
14. proponer mejoras.

## Principio de ejecución

El sistema debe priorizar siempre:

**ANALIZAR → HACER → COMPROBAR → CORREGIR → VALIDAR → CONTINUAR**

No se debe declarar terminado un proyecto únicamente porque la documentación esté completa.

El objetivo final es un proyecto funcional y validado.

## Modo de trabajo

`MODO-TRABAJO.md` define el comportamiento operativo de ChatGPT durante las sesiones de trabajo.

Cuando el usuario active el modo de trabajo, ChatGPT debe continuar autónomamente mientras pueda avanzar con las herramientas disponibles.

Debe detenerse únicamente cuando exista un bloqueo real que requiera una acción manual del usuario o cuando sea necesaria una decisión que no pueda determinarse de forma fiable.

## Evolución mediante pruebas reales

Los fixtures permiten probar el sistema de forma controlada.

Los proyectos reales permiten descubrir limitaciones que no aparecen en la documentación teórica.

Cuando una prueba o proyecto real revele un problema de metodología, documentación, automatización, integración o ejecución, el sistema debe incorporar la mejora correspondiente para que futuras ejecuciones sean mejores.

## Regla de fuente de verdad

La documentación del repositorio y el estado real de los archivos tienen prioridad sobre suposiciones o memoria conversacional.

Antes de modificar la arquitectura debe comprobarse el estado real del repositorio.

## Estado

BASE-PROYECTOS se encuentra en fase de auditoría, mejora y validación mediante pruebas progresivas.

El objetivo es acercar progresivamente el sistema a un proceso de ejecución reproducible, automatizable y fiable de principio a fin.


