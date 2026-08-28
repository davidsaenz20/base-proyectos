# ESTADO DEL PROYECTO

> Estado operativo actual de BASE-PROYECTOS.
>
> Este archivo es la fuente de verdad sobre dónde estamos, qué está terminado, qué está pendiente y cuál es el siguiente trabajo.
>
> Debe mantenerse sincronizado con el estado real del repositorio.

---

# 1. ESTADO ACTUAL

**Proyecto:** BASE-PROYECTOS

**Estado:** En desarrollo

**Fase actual:** Fase 1 — Consolidación y validación de la BASE

**Objetivo actual:** Consolidar la arquitectura documental, comprobar la coherencia entre todas las capas y validar que BASE-PROYECTOS pueda utilizarse realmente antes de iniciar un proyecto real.

**Última actualización:** 2026-08-28

---

# 2. ÚLTIMO PUNTO VÁLIDO

Se ha realizado una revisión de la arquitectura general y de las principales capas documentales de BASE-PROYECTOS.

Se considera completada la auditoría inicial de:

- `00-CONTROL/`;
- `04-TIPOS-PROYECTO/`.

También se han revisado de forma estructural:

- `01-UNIVERSAL/`;
- `02-MODULOS/`;
- `03-PLANTILLAS/`;
- `05-FIXTURES/`;
- `06-PROYECTOS/`.

Se han incorporado o revisado fixtures específicos para:

- WEB DE AFILIACIÓN;
- DIRECTORIO-LOCAL.

El protocolo de pruebas establece que las especializaciones que introducen comportamiento, requisitos, módulos, validaciones, riesgos, dependencias o reglas propias deben disponer de cobertura específica.

Se ha creado y definido `MODO-TRABAJO.md` en la raíz del repositorio para establecer el protocolo de trabajo autónomo entre el usuario y ChatGPT.

El trabajo ya no debe volver a comenzar por la auditoría individual de `00-CONTROL/`, salvo que una auditoría posterior detecte una inconsistencia que obligue a revisarlo.

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

## Control

**Estado:** Auditoría inicial completada

Se han comprobado los principales documentos de control y su función dentro del sistema.

Documentos principales:

- `README.md`;
- `ESTADO.md`;
- `ROADMAP.md`;
- `DECISIONES.md`;
- `REGLAS.md`;
- `INVENTARIO-DOCUMENTOS.md`.

El sistema de control debe utilizarse como fuente de verdad operativa, pero sus documentos deben mantenerse sincronizados entre sí.

---

## Tipos de proyecto

**Estado:** Auditoría inicial completada

Se ha revisado la estructura de `04-TIPOS-PROYECTO/`.

Se han comprobado los tipos y especializaciones actualmente definidos.

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

Las especializaciones que introducen comportamiento propio deben disponer de cobertura específica mediante fixtures.

---

## Fixtures

**Estado:** Estructurados

Se han incorporado o actualizado fixtures para comprobar comportamientos específicos.

Fixtures revisados:

- `05-FIXTURES/proyecto-web-afiliacion.md`;
- `05-FIXTURES/proyecto-directorio-local.md`.

La existencia de un fixture no implica por sí sola que el comportamiento esté validado.

La validación real debe ejecutarse posteriormente.

---

## Protocolo de pruebas

**Estado:** Actualizado

Se ha actualizado:

`05-FIXTURES/PROTOCOLO-PRUEBAS.md`

El protocolo establece una regla específica para determinar cuándo una especialización necesita un fixture propio y cuándo puede quedar cubierta por el fixture de su tipo base.

---

## Modo de trabajo

**Estado:** Definido

Existe:

`MODO-TRABAJO.md`

Su objetivo es permitir trabajo autónomo por bloques y utilizar `.` como comando rápido de continuación.

El modo de trabajo debe permitir:

- comprobar el estado real antes de continuar;
- recuperar el último punto válido;
- trabajar de forma autónoma;
- evitar pedir confirmaciones innecesarias;
- detenerse únicamente cuando sea necesaria la intervención del usuario;
- identificar claramente cuándo el usuario debe modificar un archivo;
- entregar el contenido completo del archivo cuando sea necesaria una modificación manual;
- entregar dicho contenido en una única caja copiable;
- comprobar posteriormente que la modificación existe realmente en GitHub;
- evitar ciclos de mensajes en los que el usuario tenga que enviar puntos sin que exista una acción real pendiente;
- utilizar una vía alternativa de acceso cuando la vía principal no permita comprobar el repositorio.

---

# 4. PROBLEMAS IDENTIFICADOS

## Problema 1 — Estado operativo desactualizado

`00-CONTROL/ESTADO.md` estaba indicando como siguiente tarea la auditoría completa de `00-CONTROL/`, aunque esa auditoría ya había sido realizada.

**Consecuencia:**

El sistema podía recuperar un punto de trabajo anterior y repetir tareas ya realizadas.

**Acción:**

Este archivo se actualiza para establecer como siguiente punto la auditoría cruzada de toda la BASE.

---

## Problema 2 — Roadmap pendiente de sincronización

`00-CONTROL/ROADMAP.md` contiene las fases generales del trabajo, pero debe comprobarse contra el estado real de la BASE.

**Consecuencia:**

El roadmap puede describir correctamente el proceso general sin reflejar con suficiente precisión el punto operativo actual.

**Acción:**

Auditar el roadmap contra el estado real después de completar la comprobación cruzada.

---

## Problema 3 — Auditoría cruzada pendiente

Las diferentes capas han sido revisadas parcialmente, pero todavía no se ha completado una auditoría cruzada exhaustiva.

Debe comprobarse que:

- las rutas existen;
- las referencias entre documentos son correctas;
- los tipos están conectados con sus módulos;
- los tipos están conectados con sus plantillas;
- las especializaciones están cubiertas;
- los fixtures corresponden a los comportamientos que deben probar;
- no existen reglas contradictorias;
- no existen documentos obsoletos;
- el estado coincide con el repositorio real.

---

## Problema 4 — Validación funcional pendiente

La documentación y los fixtures existen, pero todavía falta demostrar mediante pruebas reales que las reglas producen los resultados esperados.

**Consecuencia:**

Una BASE documentalmente correcta puede contener errores que solo aparezcan al intentar utilizarla.

**Acción:**

Ejecutar validaciones reales mediante los fixtures antes de considerar la BASE terminada.

---

## Problema 5 — Porcentajes de progreso

Los porcentajes históricos incluidos en este archivo eran estimaciones aproximadas y no estaban respaldados por una métrica suficientemente objetiva.

**Acción:**

A partir de ahora, los porcentajes deben utilizarse como indicadores de avance funcional por área y no como porcentaje de archivos existentes.

El porcentaje global solo debe modificarse cuando exista evidencia suficiente para justificar el cambio.

No debe utilizarse una media simple de archivos.

---

# 5. TRABAJO PENDIENTE

## Prioridad 1 — Auditoría cruzada de la BASE

Comprobar conjuntamente:

- `00-CONTROL/`;
- `01-UNIVERSAL/`;
- `02-MODULOS/`;
- `03-PLANTILLAS/`;
- `04-TIPOS-PROYECTO/`;
- `05-FIXTURES/`;
- `06-PROYECTOS/`.

Objetivo:

Determinar si todas las capas son coherentes entre sí.

---

## Prioridad 2 — Sincronización del sistema de control

Después de la auditoría cruzada:

- actualizar `ESTADO.md`;
- actualizar `ROADMAP.md` si es necesario;
- actualizar `INVENTARIO-DOCUMENTOS.md` si es necesario;
- registrar decisiones nuevas en `DECISIONES.md` si procede.

---

## Prioridad 3 — Validación real mediante fixtures

Ejecutar pruebas reales sobre los fixtures disponibles.

Objetivo:

Comprobar que:

- las entradas son interpretadas correctamente;
- las reglas se aplican;
- los módulos adecuados son seleccionados;
- las plantillas adecuadas son seleccionadas;
- los tipos de proyecto se comportan como corresponde;
- las especializaciones reciben su tratamiento específico;
- los errores se detectan;
- los resultados pueden verificarse.

---

## Prioridad 4 — Corrección de errores encontrados

Cuando una validación detecte un problema:

1. identificar el origen;
2. determinar qué documento o componente es responsable;
3. corregirlo;
4. volver a ejecutar la validación afectada;
5. comprobar que no se ha introducido una contradicción;
6. actualizar el estado.

---

## Prioridad 5 — Proyecto real de prueba

Solo cuando la BASE haya superado la validación funcional:

Iniciar un proyecto real utilizando exclusivamente el sistema construido.

El proyecto real servirá como prueba definitiva de que la BASE permite pasar desde una necesidad inicial hasta un resultado funcional.

---

# 6. SIGUIENTE TAREA

La siguiente tarea lógica es:

**AUDITORÍA CRUZADA DE TODA LA BASE.**

Orden previsto:

1. comprobar la estructura real del repositorio;
2. comprobar `00-CONTROL`;
3. comprobar `01-UNIVERSAL`;
4. comprobar `02-MODULOS`;
5. comprobar `03-PLANTILLAS`;
6. comprobar `04-TIPOS-PROYECTO`;
7. comprobar `05-FIXTURES`;
8. comprobar `06-PROYECTOS`;
9. cruzar referencias entre capas;
10. detectar contradicciones;
11. detectar archivos faltantes u obsoletos;
12. determinar correcciones necesarias;
13. actualizar `ESTADO.md`;
14. actualizar `ROADMAP.md` si procede;
15. establecer un nuevo punto válido.

No repetir auditorías ya completadas salvo que una dependencia o inconsistencia descubierta posteriormente obligue a revisarlas.

---

# 7. BLOQUEOS

**Bloqueo actual:** Ninguno conocido.

**Intervención del usuario necesaria:**

Únicamente cuando sea necesario:

- modificar manualmente un archivo;
- copiar contenido proporcionado por ChatGPT al repositorio;
- realizar una acción externa que el sistema no pueda ejecutar;
- proporcionar información imprescindible que no exista en el repositorio.

Si una herramienta de acceso al repositorio falla, debe intentarse una vía alternativa.

Repositorio público de respaldo:

`https://github.com/davidsaenz20/base-proyectos.git`

La imposibilidad temporal de utilizar una vía de acceso no debe interpretarse automáticamente como un problema del proyecto.

Debe intentarse una vía alternativa antes de declarar el trabajo bloqueado.

Si tampoco es posible recuperar la información necesaria, declarar explícitamente:

**BLOQUEADO — ACCESO O LECTURA INSUFICIENTE**

No inventar contenido.

---

# 8. CRITERIO PARA CONTINUAR

Después de cada modificación relevante:

1. comprobar que el archivo existe;
2. comprobar que la ruta es correcta;
3. comprobar que el contenido está actualizado;
4. comprobar que no se ha perdido contenido necesario;
5. comprobar que las referencias relacionadas siguen siendo válidas;
6. actualizar este archivo si cambia el estado;
7. determinar automáticamente la siguiente tarea.

No considerar una modificación realizada simplemente porque el usuario indique que la ha subido.

Debe verificarse en el repositorio siempre que sea técnicamente posible.

Si un archivo puede leerse pero su contenido completo no puede recuperarse de forma fiable:

**BLOQUEADO — LECTURA INCOMPLETA**

No sobrescribir el archivo mediante una reconstrucción parcial.

---

# 9. PROGRESO FUNCIONAL

Los porcentajes representan una estimación del avance funcional de cada área.

No representan el porcentaje de archivos creados.

| Área | Progreso |
|---|---:|
| Arquitectura | 90% |
| Control | 90% |
| Universal | 60% |
| Módulos | 50% |
| Plantillas | 50% |
| Tipos de proyecto | 90% |
| Fixtures | 75% |
| Protocolo de pruebas | 80% |
| Documentación | 80% |
| Auditoría cruzada | 20% |
| Validación funcional | 5% |
| Construcción | 0% |
| **TOTAL BASE** | **≈65%** |

Estos porcentajes son indicadores operativos y pueden cambiar cuando una auditoría o validación aporte evidencia nueva.

El porcentaje global no debe calcularse como una media simple de archivos.

Debe representar el avance funcional aproximado hacia una BASE:

- coherente;
- validada;
- reutilizable;
- ejecutable;
- mantenible;
- utilizable para construir proyectos reales.

Si no existe evidencia suficiente para modificar un porcentaje, debe mantenerse el último valor válido.

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
- validación;
- arquitectura;
- punto de recuperación.

No actualizarlo por cada acción trivial.

Su función es permitir recuperar el trabajo incluso si el contexto de la conversación deja de estar disponible.

---

# 11. SIGUIENTE PUNTO DE RECUPERACIÓN

Si se pierde el contexto de la conversación, comenzar desde:

**Proyecto:** BASE-PROYECTOS

**Fase:** Fase 1 — Consolidación y validación de la BASE

**Área:** Auditoría cruzada de la BASE

**Último bloque completado:**

- revisión inicial de `00-CONTROL/`;
- auditoría inicial de `04-TIPOS-PROYECTO/`;
- revisión estructural de `01-UNIVERSAL/`;
- revisión estructural de `02-MODULOS/`;
- revisión estructural de `03-PLANTILLAS/`;
- revisión estructural de `05-FIXTURES/`;
- revisión estructural de `06-PROYECTOS/`;
- actualización del protocolo de pruebas para especializaciones;
- incorporación/revisión de fixtures específicos.

**Siguiente acción:**

Realizar la auditoría cruzada de todas las capas y determinar las correcciones necesarias antes de iniciar la validación funcional.

No volver automáticamente a auditar `00-CONTROL/` como tarea principal.

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

El inventario documental pertenece a:

`00-CONTROL/INVENTARIO-DOCUMENTOS.md`

Las decisiones estructurales pertenecen a:

`00-CONTROL/DECISIONES.md`

Este archivo debe mantenerse sincronizado con el estado real del repositorio.

Nunca debe utilizarse para justificar que una tarea está terminada si no existe evidencia suficiente.

Nunca debe inventarse un estado para evitar un bloqueo.

Nunca debe reconstruirse parcialmente un archivo que no pueda recuperarse de forma fiable.

El objetivo del sistema de estado es permitir continuar el trabajo de forma autónoma, verificable y recuperable.


