FLUJO DE EJECUCIÓN DE PROYECTO

PROPÓSITO

Definir el proceso general que debe seguir un proyecto desde su inicio hasta su funcionamiento real en producción.

Este documento define cómo se ejecuta un proyecto.

No sustituye:

- "01-UNIVERSAL/PROTOCOLO-EJECUCION.md" → define el comportamiento operativo de la IA.
- "00-CONTROL/ESTADO.md" → define dónde está actualmente el proyecto.
- "03-PLANTILLAS/ROADMAP.md" → define el plan específico del proyecto.

---

REGLA GENERAL DE EJECUCIÓN

Cada fase debe seguir este ciclo:

ENTRADA → ANÁLISIS/TRABAJO → ENTREGABLE → VALIDACIÓN → ACTUALIZACIÓN DE ESTADO → AVANCE

No se debe avanzar a la siguiente fase mientras el criterio de salida de la fase actual no esté cumplido.

Crear un archivo, completar una plantilla o realizar una configuración no significa que el trabajo esté terminado.

Debe existir evidencia suficiente de que el resultado cumple su objetivo.

---

FUENTE DE VERDAD

Durante la ejecución:

- "ESTADO.md" determina la fase y paso actuales.
- "ROADMAP.md" determina el trabajo específico planificado.
- Este documento determina el flujo general y los criterios de las fases.
- Las plantillas determinan la estructura de los entregables.
- El protocolo de ejecución determina cómo debe actuar la IA.

Si existe una contradicción, la IA debe detenerse y resolverla antes de continuar.

---

FASE 1 — ENTRADA

Objetivo

Comprender qué quiere conseguir el usuario.

Entrada

Puede existir:

- necesidad;
- problema;
- idea;
- petición;
- documentación;
- proyecto existente;
- automatización existente.

Acciones

1. Leer la petición.
2. Identificar el objetivo.
3. Identificar el problema.
4. Identificar al usuario o usuarios.
5. Identificar el resultado esperado.
6. Detectar información desconocida.
7. Determinar si existe información suficiente para comenzar el análisis.

Entregable

Primera descripción estructurada del proyecto.

Validación

Debe quedar claro:

- qué se quiere conseguir;
- qué problema se pretende resolver;
- para quién;
- cuál es el resultado esperado.

Para avanzar

Si falta información crítica, preguntar.

Si la información es suficiente, registrar la salida y pasar a Fase 2.

---

FASE 2 — ANÁLISIS

Objetivo

Determinar qué necesita realmente el proyecto.

Entrada

Resultado validado de Fase 1.

Acciones

Analizar:

- problema;
- usuarios;
- entradas;
- procesos;
- salidas;
- integraciones;
- datos;
- restricciones;
- riesgos;
- costes relevantes;
- información desconocida.

Entregable

Análisis inicial validado.

Validación

Debe existir una comprensión suficiente del problema y de sus restricciones para tomar decisiones de definición.

Para avanzar

No tomar decisiones críticas basadas en información desconocida.

Si falta información crítica, preguntar.

---

FASE 3 — CLASIFICACIÓN

Objetivo

Determinar qué tipo o tipos de proyecto se están construyendo.

Entrada

Análisis inicial.

Acciones

1. Consultar "04-TIPOS-PROYECTO".
2. Comparar el proyecto con los tipos disponibles.
3. Seleccionar el tipo o tipos adecuados.
4. Consultar fixtures relacionados cuando sean útiles.
5. Utilizar los fixtures únicamente como referencia.
6. No copiar datos ficticios al proyecto real.

Entregable

Clasificación del proyecto.

Validación

Debe existir una justificación suficiente de la clasificación elegida.

Para avanzar

El tipo de proyecto debe estar identificado o documentarse por qué no encaja en los tipos existentes.

Si falta una categoría reutilizable, registrarla como necesidad antes de continuar.

---

FASE 4 — DEFINICIÓN

Objetivo

Convertir la idea y el análisis en una definición concreta y verificable.

Entrada

Fases 1–3 validadas.

Acciones

Completar la plantilla de proyecto con:

- identificación;
- objetivo;
- problema;
- usuarios;
- propuesta;
- alcance;
- fuera de alcance;
- requisitos iniciales;
- módulos;
- tecnología inicial;
- arquitectura inicial;
- datos;
- riesgos;
- decisiones;
- roadmap;
- criterios de éxito;
- validación.

Entregable

"definicion.md"

Validación

Debe quedar definido como mínimo:

- qué se construye;
- para quién;
- qué problema resuelve;
- qué incluye;
- qué no incluye;
- qué requisitos debe cumplir;
- cómo se sabrá si funciona.

Para avanzar

No comenzar el diseño técnico si el objetivo, alcance o requisitos críticos siguen siendo ambiguos.

---

FASE 5 — SELECCIÓN DE MÓDULOS

Objetivo

Determinar qué capacidades reutilizables necesita el proyecto.

Entrada

Definición validada.

Acciones

1. Consultar "02-MODULOS".
2. Identificar módulos necesarios.
3. Seleccionar únicamente los necesarios.
4. Detectar capacidades inexistentes.
5. Si una capacidad debe ser reutilizable, documentarla como módulo.
6. Registrar excepciones específicas del proyecto.

Entregable

Lista de módulos seleccionados y capacidades necesarias.

Validación

Cada módulo seleccionado debe tener una función concreta dentro del proyecto.

Para avanzar

No deben quedar capacidades críticas sin resolver o identificadas como pendientes.

---

FASE 6 — REQUISITOS

Objetivo

Definir exactamente qué debe hacer el sistema.

Entrada

Definición y módulos seleccionados.

Acciones

Documentar:

Requisitos funcionales

Qué debe hacer el sistema.

Requisitos técnicos

Qué condiciones técnicas debe cumplir.

Requisitos no funcionales

Rendimiento, disponibilidad, escalabilidad, mantenibilidad y otras condiciones relevantes.

Integraciones

Servicios, APIs, plataformas y sistemas externos.

Datos

Qué datos recibe, procesa, almacena y produce.

Seguridad

Autenticación, autorización, secretos, privacidad y protección de datos cuando corresponda.

Entregable

"requisitos.md"

Validación

Cada requisito crítico debe ser:

- comprensible;
- verificable;
- suficientemente concreto.

Para avanzar

No pasar a arquitectura con requisitos críticos ambiguos.

---

FASE 7 — ARQUITECTURA

Objetivo

Diseñar cómo funcionará el sistema.

Entrada

Requisitos validados.

Acciones

Definir:

- componentes;
- servicios;
- APIs;
- bases de datos;
- automatizaciones;
- flujo de información;
- autenticación;
- autorización;
- seguridad;
- almacenamiento;
- observabilidad;
- dependencias externas;
- recuperación ante errores.

Entregable

"arquitectura.md"

Validación

La arquitectura debe:

- cumplir los requisitos;
- ser técnicamente viable;
- ser suficientemente sencilla;
- contemplar seguridad;
- contemplar errores;
- poder desplegarse en la realidad.

Para avanzar

No construir componentes cuya arquitectura crítica todavía no esté resuelta.

---

FASE 8 — PLANIFICACIÓN

Objetivo

Convertir la definición y arquitectura en un plan ejecutable.

Entrada

Arquitectura validada.

Acciones

1. Crear o actualizar el roadmap específico.
2. Dividir el trabajo en tareas.
3. Ordenar dependencias.
4. Identificar bloqueos.
5. Definir criterios de finalización.
6. Identificar entregables.
7. Establecer el siguiente paso concreto.
8. Preparar el estado inicial de ejecución.

Entregable

"roadmap.md"

y estado operativo inicial en:

"00-CONTROL/ESTADO.md"

Validación

Cada bloque importante del trabajo debe tener:

- objetivo;
- tareas;
- entregable;
- criterio de finalización;
- dependencias cuando existan.

Para avanzar

Debe existir un primer paso ejecutable sin necesidad de improvisar.

---

FASE 9 — CONSTRUCCIÓN

Objetivo

Construir el sistema definido.

Entrada

Planificación validada.

Acciones

Implementar:

- componentes;
- servicios;
- integraciones;
- automatizaciones;
- APIs;
- datos;
- configuración;
- seguridad.

Regla

Trabajar siguiendo el paso actual registrado en "ESTADO.md".

No saltar a tareas posteriores por iniciativa propia.

Entregable

Primera versión funcional.

Validación

Cada componente importante debe comprobarse individualmente y dentro del flujo correspondiente.

Para avanzar

Debe existir una versión funcional suficiente para realizar pruebas.

---

FASE 10 — PRUEBAS

Objetivo

Comprobar que el sistema funciona técnicamente.

Entrada

Primera versión funcional.

Acciones

Realizar las pruebas necesarias:

- funcionales;
- integración;
- errores;
- seguridad;
- rendimiento cuando sea necesario;
- compatibilidad;
- regresión.

Registrar:

- prueba;
- objetivo;
- resultado esperado;
- resultado obtenido;
- estado;
- error;
- corrección;
- nueva prueba cuando corresponda.

Entregable

Resultados de testing.

Validación

Los errores críticos deben estar corregidos o existir una decisión explícita y documentada sobre ellos.

Para avanzar

El sistema debe superar las pruebas necesarias para poder validarse como solución.

---

FASE 11 — VALIDACIÓN

Objetivo

Determinar si el proyecto resuelve realmente el problema para el que fue creado.

Entrada

Sistema probado.

Acciones

Comprobar:

1. objetivo;
2. requisitos;
3. funcionamiento;
4. seguridad;
5. integraciones;
6. experiencia del usuario;
7. costes;
8. estabilidad;
9. criterios de éxito.

Regla

Un sistema técnicamente funcional que no resuelve el problema real no se considera terminado.

Entregable

"validacion.md"

Validación

Debe existir evidencia suficiente de que el sistema cumple el objetivo.

Para avanzar

El proyecto debe estar preparado para despliegue real.

---

FASE 12 — DESPLIEGUE

Objetivo

Poner el sistema en funcionamiento real.

Entrada

Sistema validado.

Acciones

Configurar:

- entorno de producción;
- dominio cuando corresponda;
- servidores;
- credenciales;
- variables de entorno;
- servicios externos;
- copias de seguridad;
- recuperación;
- permisos;
- configuración final;
- monitorización.

Comprobaciones previas

- configuración;
- seguridad;
- secretos;
- backups;
- monitorización;
- recuperación ante errores.

Entregable

Sistema desplegado.

Validación

Debe poder accederse al sistema en su entorno real.

Para avanzar

El despliegue debe estar realizado y preparado para operaciones reales controladas.

---

FASE 13 — VALIDACIÓN EN PRODUCCIÓN

Objetivo

Comprobar el funcionamiento del sistema real en su entorno real.

Entrada

Sistema desplegado.

Acciones

Ejecutar operaciones reales controladas y comprobar:

- entradas;
- procesamiento;
- salidas;
- errores;
- notificaciones;
- registros;
- integraciones;
- recuperación.

Entregable

Evidencias de funcionamiento real.

Validación

El flujo real debe funcionar de extremo a extremo.

Para avanzar

No considerar el proyecto terminado si solamente funciona en pruebas o entorno de desarrollo.

---

FASE 14 — MONITORIZACIÓN

Objetivo

Detectar problemas después del despliegue.

Entrada

Sistema funcionando en producción.

Acciones

Monitorizar, cuando corresponda:

- disponibilidad;
- errores;
- rendimiento;
- ejecuciones;
- consumo;
- costes;
- integraciones;
- eventos importantes.

Definir también:

- qué se vigila;
- cómo se detecta;
- qué ocurre ante un error;
- quién debe actuar;
- cómo se recupera el servicio.

Entregable

Sistema monitorizado y procedimiento básico de actuación.

Validación

Debe existir una forma realista de detectar los problemas relevantes.

Para avanzar

La operación debe ser suficientemente controlable para considerar estable el proyecto.

---

FASE 15 — CIERRE

Objetivo

Determinar que el proyecto ha cumplido su objetivo y puede considerarse terminado.

Comprobaciones finales

- objetivo cumplido;
- requisitos validados;
- pruebas superadas;
- seguridad revisada;
- sistema desplegado;
- funcionamiento real comprobado;
- monitorización disponible;
- evidencias conservadas;
- documentación actualizada;
- decisiones importantes registradas;
- incidencias críticas resueltas o aceptadas explícitamente.

Entregable

Proyecto cerrado y documentación final actualizada.

Estado final

El proyecto solo puede marcarse como:

TERMINADO

cuando los criterios anteriores estén cumplidos.

El "ESTADO.md" debe reflejar:

Estado: Terminado

Progreso: 100 %

---

REGLAS DE EJECUCIÓN PARA LA IA

La IA debe:

1. Leer el protocolo general antes de ejecutar.
2. Leer el estado actual del proyecto.
3. Identificar el paso actual.
4. Consultar únicamente la documentación necesaria para ese paso.
5. Consultar las plantillas correspondientes.
6. Consultar los módulos necesarios.
7. Consultar el tipo de proyecto cuando corresponda.
8. Mantener separada la información general de la información específica del proyecto.
9. No inventar información desconocida.
10. Preguntar cuando falten datos críticos.
11. Ejecutar únicamente el trabajo correspondiente al paso actual.
12. No cambiar de fase por iniciativa propia.
13. No confundir una mejora con un bloqueo.
14. Registrar los bloqueos reales.
15. Registrar las decisiones importantes.
16. Crear o actualizar el entregable correspondiente.
17. Validar el resultado antes de avanzar.
18. Actualizar "ESTADO.md".
19. Mantener actualizado el roadmap cuando cambie el plan.
20. No considerar terminado un trabajo únicamente porque exista un archivo.
21. No considerar terminado un sistema que no haya sido probado.
22. No considerar terminado el proyecto hasta comprobar su funcionamiento real.
23. Si detecta una necesidad fuera del paso actual que no sea un bloqueo, registrarla y continuar.
24. Si detecta una contradicción entre documentos, detenerse y resolverla antes de continuar.

---

REGLA PARA "SIGUE"

Cuando el usuario indique:

"Sigue"

la IA debe:

1. recuperar el estado persistente;
2. identificar la fase y paso actuales;
3. comprobar el entregable pendiente;
4. ejecutar el siguiente trabajo correspondiente al paso actual;
5. validar;
6. actualizar el estado;
7. continuar únicamente si el criterio de avance está cumplido.

"Sigue" no autoriza a cambiar de fase, introducir una nueva metodología ni iniciar trabajo no relacionado con el paso actual.

---

REGLA DE BLOQUEO

Se considera bloqueo únicamente aquello que impide completar el paso actual.

No son bloqueos por sí mismos:

- ideas nuevas;
- mejoras;
- optimizaciones;
- alternativas tecnológicas;
- refactorizaciones;
- documentación no necesaria para el paso actual.

Una mejora pendiente no permite cambiar de fase ni desviarse del plan.

---

REGLA DE RETROCESO

No se retrocede de fase salvo que exista un bloqueo o una validación que demuestre que una decisión anterior impide continuar.

Si es necesario retroceder:

1. identificar la causa;
2. documentarla;
3. actualizar "ESTADO.md";
4. indicar qué fase debe revisarse;
5. resolver el problema;
6. volver al flujo normal.

---

PRINCIPIO FINAL

Pensar → definir → diseñar → planificar → construir → probar → validar → desplegar → comprobar en producción → monitorizar → cerrar.

El objetivo final no es producir documentación.

El objetivo final es:

CONSTRUIR ALGO QUE FUNCIONE REALMENTE.
