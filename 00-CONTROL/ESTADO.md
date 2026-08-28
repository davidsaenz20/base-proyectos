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

Se ha realizado una revisión de la arquitectura general, documentación de control, tipos de proyecto, fixtures y sistema de trabajo.

La auditoría de `04-TIPOS-PROYECTO/` se considera completada en esta etapa.

Se ha comprobado la existencia y coherencia de los tipos principales y de las especializaciones actualmente identificadas.

También se han incorporado fixtures específicos para:

- WEB DE AFILIACIÓN;
- DIRECTORIO-LOCAL.

El protocolo de pruebas ha sido actualizado para establecer una regla de cobertura específica para especializaciones.

Se ha creado y definido `MODO-TRABAJO.md` en la raíz del repositorio para establecer el protocolo de trabajo autónomo entre el usuario y ChatGPT.

---

# 3. TRABAJO COMPLETADO

## Arquitectura general

**Estado:** Avanzado

La estructura principal de BASE-PROYECTOS está definida y organizada por capas.

---

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

---

## Tipos de proyecto

**Estado:** Auditoría inicial completada

Se ha revisado la estructura de `04-TIPOS-PROYECTO/`.

Se ha comprobado la existencia de los tipos y especializaciones actualmente definidos.

Entre ellos:

- WEB;
- WEB DE AFILIACIÓN;
- APP MÓVIL;
- SaaS;
- Ecommerce;
- API / Servicio;
- Automatización;
- Asistente IA;
- Directorio;
- DIRECTORIO-LOCAL;
- Portal.

Las especializaciones que introducen comportamiento propio disponen de cobertura específica mediante fixtures.

---

## Fixtures

**Estado:** Estructurados

Se han incorporado o actualizado fixtures para comprobar comportamientos específicos.

Fixtures revisados:

- `05-FIXTURES/proyecto-web-afiliacion.md`
- `05-FIXTURES/proyecto-directorio-local.md`

---

## Protocolo de pruebas

**Estado:** Actualizado

Se ha actualizado:

`05-FIXTURES/PROTOCOLO-PRUEBAS.md`

El protocolo incluye ahora una regla específica para determinar cuándo una especialización necesita un fixture propio y cuándo puede quedar cubierta por el fixture de su tipo base.

---

## Modo de trabajo

**Estado:** Definido

Se ha creado:

`MODO-TRABAJO.md`

Su objetivo es permitir trabajo autónomo por bloques y utilizar `.` como comando rápido de continuación.

El modo de trabajo debe permitir:

- comprobar el estado real antes de continuar;
- recuperar el último punto válido;
- trabajar de forma autónoma;
- detenerse únicamente cuando sea necesaria la intervención del usuario;
- identificar claramente cuándo el usuario debe modificar un archivo;
- comprobar posteriormente que la modificación existe realmente en GitHub;
- evitar ciclos de mensajes en los que el usuario tenga que enviar puntos sin que exista una acción real pendiente.

---

## Historial

**Estado:** Revisado

Se ha revisado el historial reciente del repositorio y de trabajo para reconstruir el estado operativo.

---

# 4. PROBLEMAS IDENTIFICADOS

## Problema 1 — Estado operativo desactualizado

`00-CONTROL/ESTADO.md` no estaba reflejando correctamente los avances realizados.

**Consecuencia:** el sistema podía recuperar un punto de trabajo anterior aunque algunas tareas ya hubieran sido completadas.

**Acción:** actualizar este archivo para convertirlo en una fuente persistente y actualizada del estado operativo.

---

## Problema 2 — Roadmap incompleto

`00-CONTROL/ROADMAP.md` contiene las fases generales, pero todavía necesita convertirse en un roadmap específico del trabajo actual.

**Consecuencia:** define el proceso general, pero no determina con suficiente precisión las tareas, dependencias e hitos concretos.

**Acción:** auditar y completar el roadmap después de actualizar el estado.

---

## Problema 3 — Cobertura de especializaciones

Se detectó que la existencia de un tipo base no garantiza que sus especializaciones estén realmente cubiertas.

**Acción realizada:** actualizar `PROTOCOLO-PRUEBAS.md` para exigir cobertura específica cuando una especialización introduzca comportamiento, requisitos, módulos, validaciones, riesgos, dependencias o reglas propias.

---

# 5. TRABAJO PENDIENTE

## Prioridad 1

Auditar completamente `00-CONTROL/`.

Comprobar:

- README;
- ESTADO;
- ROADMAP;
- DECISIONES;
- REGLAS;
- INVENTARIO;
- cualquier documento relacionado.

Objetivo:

Conseguir un sistema de control coherente, actualizado y recuperable.

---

## Prioridad 2

Completar el roadmap específico.

Debe determinar:

- objetivo actual;
- fases;
- tareas;
- dependencias;
- hitos;
- criterios de finalización;
- orden de ejecución.

---

## Prioridad 3

Realizar auditoría global de coherencia.

Comprobar que:

- los documentos se referencian correctamente;
- no existen reglas contradictorias;
- no faltan componentes necesarios;
- no existen archivos obsoletos;
- los tipos de proyecto están correctamente conectados con sus módulos;
- los fixtures cubren los comportamientos necesarios;
- el sistema de trabajo coincide con el estado real;
- la estructura responde al objetivo de BASE-PROYECTOS.

---

## Prioridad 4

Iniciar validación real de la BASE mediante los fixtures disponibles.

Objetivo:

Comprobar que las reglas documentadas no solo existen, sino que permiten obtener resultados correctos y detectar errores.

---

# 6. SIGUIENTE TAREA

La siguiente tarea lógica es:

**AUDITAR `00-CONTROL/` COMPLETAMENTE.**

La auditoría de `04-TIPOS-PROYECTO/` ya está completada en este bloque y no debe volver a considerarse la siguiente tarea salvo que la auditoría de control encuentre una inconsistencia que obligue a revisarla.

Orden previsto:

1. auditar `00-CONTROL/README.md`;
2. auditar `00-CONTROL/ESTADO.md`;
3. auditar `00-CONTROL/ROADMAP.md`;
4. auditar documentos de decisiones y reglas;
5. comprobar referencias cruzadas;
6. actualizar lo necesario;
7. establecer el siguiente punto válido.

---

# 7. BLOQUEOS

**Bloqueo actual:** Ninguno.

**Intervención del usuario necesaria:** Únicamente cuando sea necesario modificar manualmente un archivo o realizar una acción que no pueda ejecutar el sistema.

Si una herramienta de acceso al repositorio falla, debe utilizarse como alternativa la URL pública del repositorio:

`https://github.com/davidsaenz20/base-proyectos.git`

La imposibilidad temporal de utilizar una vía de acceso no debe interpretarse automáticamente como un problema del proyecto.

Debe intentarse una vía alternativa antes de declarar el trabajo bloqueado.

---

# 8. CRITERIO PARA CONTINUAR

Después de cada modificación relevante:

1. comprobar que el archivo existe;
2. comprobar que la ruta es correcta;
3. comprobar que el contenido está actualizado;
4. comprobar que no se ha perdido contenido necesario;
5. actualizar este archivo si cambia el estado;
6. determinar automáticamente la siguiente tarea.

No considerar una modificación realizada simplemente porque el usuario indique que la ha subido.

Debe verificarse en el repositorio.

---

# 9. PROGRESO ESTIMADO

Estos porcentajes representan una estimación del progreso funcional del trabajo, no el porcentaje de archivos creados.

| Área | Progreso |
|---|---:|
| Arquitectura | 90% |
| Control | 50% |
| Tipos de proyecto | 90% |
| Fixtures | 75% |
| Protocolo de pruebas | 80% |
| Documentación | 80% |
| Auditoría global | 30% |
| Validación | 5% |
| Construcción | 0% |
| **TOTAL BASE** | **60%** |

Estos porcentajes pueden cambiar cuando una auditoría posterior demuestre que una parte estaba sobrevalorada o infravalorada.

El porcentaje total no debe calcularse simplemente como una media de archivos.

Debe representar el avance funcional aproximado hacia una BASE coherente, validada y utilizable.

---

# 10. REGLA DE ACTUALIZACIÓN

Este archivo debe actualizarse cuando exista un cambio significativo en:

- estado;
- fase;
- tarea;
- prioridad;
- bloqueo;
- decisión;
- progreso;
- cobertura;
- validación.

No actualizarlo por cada acción trivial.

Su función es permitir recuperar el trabajo incluso si el contexto de la conversación deja de estar disponible.

---

# 11. SIGUIENTE PUNTO DE RECUPERACIÓN

Si se pierde el contexto de la conversación, comenzar desde:

**Proyecto:** BASE-PROYECTOS

**Fase:** Fase 1 — Descubrimiento y definición de la BASE

**Área:** `00-CONTROL/`

**Tarea:** Auditoría completa del sistema de control.

**Último bloque completado:**

- auditoría inicial de `04-TIPOS-PROYECTO/`;
- actualización de `05-FIXTURES/PROTOCOLO-PRUEBAS.md`;
- incorporación/revisión de fixtures de especializaciones.

**Siguiente acción:**

Auditar `00-CONTROL/` y convertir el sistema de control en una fuente coherente y recuperable del estado del proyecto.

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

Las reglas de validación de fixtures pertenecen a:

`05-FIXTURES/PROTOCOLO-PRUEBAS.md`

Este archivo debe mantenerse sincronizado con el estado real del repositorio.


