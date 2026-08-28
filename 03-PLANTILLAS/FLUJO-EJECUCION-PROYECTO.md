FLUJO DE EJECUCIÓN DE PROYECTO

PROPÓSITO

Definir el proceso general que debe seguir un proyecto desde su inicio hasta su funcionamiento real en producción.

Este documento define cómo se ejecuta un proyecto.

No sustituye:

- "01-UNIVERSAL/PROTOCOLO-EJECUCION.md" → define el comportamiento operativo de la IA.
- "00-CONTROL/ESTADO.md" → define dónde está actualmente el proyecto.

- "03-PLANTILLAS/PLANTILLA-ROADMAP.md" → define la estructura para crear el plan específico del proyecto.
- 
- "01-UNIVERSAL/ESTUDIO-PREVIO-VIABILIDAD.md" → define el estudio previo universal cuando el proyecto lo requiera.

---

REGLA GENERAL DE EJECUCIÓN

Cada fase debe seguir este ciclo:

ENTRADA → ANÁLISIS/TRABAJO → ENTREGABLE → VALIDACIÓN → ACTUALIZACIÓN DE ESTADO → AVANCE

Además, cuando corresponda, el flujo utilizará mecanismos transversales:

CLARIFY → ANALYZE → CONVERGE

Estos mecanismos no son fases independientes.

Forman parte del proceso de control de calidad del proyecto.

No se debe avanzar a la siguiente fase mientras el criterio de salida de la fase actual no esté cumplido.

Crear un archivo, completar una plantilla o realizar una configuración no significa que el trabajo esté terminado.

Debe existir evidencia suficiente de que el resultado cumple su objetivo.

---

MECANISMOS TRANSVERSALES

CLARIFY

Propósito

Asegurar que se entiende correctamente qué quiere conseguir el usuario antes de diseñar o construir.

Preguntas que debe resolver

- ¿Cuál es el objetivo primario?
- ¿Qué problema se pretende resolver?
- ¿Quién utilizará la solución?
- ¿Cuál es el resultado esperado?
- ¿Qué está dentro del alcance?
- ¿Qué está fuera del alcance?
- ¿Qué información crítica falta?
- ¿Qué cosas no deben asumirse?

Regla

Si existe una ambigüedad crítica que pueda cambiar el proyecto, se debe resolver antes de continuar.

Resultado

Una definición suficientemente clara del objetivo y alcance inicial.

---

ANALYZE

Propósito

Comprobar que las partes del proyecto son coherentes entre sí.

Debe comprobar:

OBJETIVO → REQUISITOS → SOLUCIÓN → ARQUITECTURA → PLAN → TAREAS

Debe detectar:

- contradicciones;
- requisitos sin solución;
- tareas innecesarias;
- dependencias olvidadas;
- riesgos no considerados;
- decisiones técnicas injustificadas;
- desviaciones del objetivo;
- información desconocida que pueda afectar a decisiones críticas;
- problemas de viabilidad.

Resultado

El proyecto queda en uno de estos estados:

🟢 COHERENTE

Se puede continuar.

🟡 DUDAS

Hay información que debe investigarse o aclararse.

🔴 CONTRADICCIÓN

Debe corregirse antes de continuar.

---

CONVERGE

Propósito

Comprobar que lo construido realmente corresponde con lo definido.

Debe comparar:

LO DEFINIDO

contra

LO IMPLEMENTADO

y posteriormente:

REQUISITOS → PRUEBAS → EVIDENCIAS

Debe detectar:

- requisitos incumplidos;
- funcionalidades ausentes;
- diferencias entre diseño e implementación;
- errores;
- decisiones que hayan cambiado sin registrarse;
- partes construidas que no aportan al objetivo;
- problemas descubiertos durante las pruebas.

Resultado

🟢 CONVERGE

La implementación corresponde con lo definido y las evidencias son suficientes.

🟡 AJUSTAR

Existen diferencias menores que deben corregirse.

🔴 NO CONVERGE

La implementación no corresponde suficientemente con el proyecto definido.

No se puede cerrar el proyecto.

---

FUENTE DE VERDAD

Durante la ejecución:

- "ESTADO.md" determina la fase y paso actuales.
- "ROADMAP.md" determina el trabajo específico planificado.
- Este documento determina el flujo general y los criterios de las fases.
- Las plantillas determinan la estructura de los entregables.
- El protocolo de ejecución determina cómo debe actuar la IA.
- "ESTUDIO-PREVIO-VIABILIDAD.md" determina cómo realizar el estudio previo de viabilidad cuando corresponda.
- "DECISIONES.md" conserva las decisiones importantes.
- "MEJORAS-SISTEMA.md" conserva la evolución del sistema.
- "BENCHMARK-SISTEMA.md" conserva las comparaciones y aprendizajes externos.

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

CLARIFY

Antes de considerar comprendida la petición, ejecutar CLARIFY.

Determinar:

- objetivo primario;
- problema;
- usuario;
- resultado esperado;
- alcance inicial;
- información desconocida;
- supuestos que no deben realizarse.

Acciones

1. Leer la petición.
2. Ejecutar CLARIFY.
3. Identificar el objetivo.
4. Identificar el problema.
5. Identificar al usuario o usuarios.
6. Identificar el resultado esperado.
7. Detectar información desconocida.
8. Determinar si existe información suficiente para comenzar el análisis.

Entregable

Primera descripción estructurada del proyecto.

Validación

Debe quedar claro:

- qué se quiere conseguir;
- qué problema se pretende resolver;
- para quién;
- cuál es el resultado esperado;
- qué información crítica falta.

Para avanzar

Si falta información crítica, preguntar.

Si la información es suficiente, registrar la salida y pasar a Fase 2.

---

FASE 2 — ANÁLISIS

Objetivo

Determinar qué necesita realmente el proyecto.

Entrada

Resultado validado de Fase 1.

ANALYZE

Realizar un primer ANALYZE para comprobar que:

objetivo → problema → usuarios → resultado esperado

son coherentes.

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
- información desconocida;
- incertidumbres críticas;
- necesidad de realizar estudio previo de viabilidad.

Entregable

Análisis inicial validado.

Validación

Debe existir una comprensión suficiente del problema y de sus restricciones para determinar qué investigación y definición son necesarias.

Para avanzar

No tomar decisiones críticas basadas en información desconocida.

Si falta información crítica, preguntar o determinar si puede investigarse.

Si ANALYZE detecta una contradicción, resolverla antes de continuar.

Si por la naturaleza del proyecto existe incertidumbre significativa sobre demanda, mercado, competencia, monetización, oportunidad o viabilidad, pasar a Fase 3.

Si el proyecto no requiere un estudio previo de viabilidad, debe registrarse el motivo y pasar a Fase 4.

---

FASE 3 — ESTUDIO PREVIO DE VIABILIDAD

Objetivo

Determinar, antes de comprometer recursos importantes en la construcción, si existe una oportunidad suficientemente razonable y cómo podría mejorarse la viabilidad de la propuesta.

Esta fase es especialmente importante para proyectos empresariales, productos, servicios, webs comerciales, aplicaciones, SaaS, plataformas, automatizaciones comerciales, sistemas de IA y cualquier proyecto cuya construcción pueda implicar una inversión significativa.

Entrada

Análisis inicial validado de Fase 2.

Acciones

Consultar:

"01-UNIVERSAL/ESTUDIO-PREVIO-VIABILIDAD.md"

Realizar un estudio exhaustivo y proporcional al proyecto.

Analizar, cuando corresponda:

- problema;
- usuario;
- demanda;
- mercado;
- tendencias;
- competencia directa;
- competencia indirecta;
- sustitutos;
- soluciones existentes;
- diferenciación;
- propuesta de valor;
- modelos de negocio;
- monetización;
- costes;
- adquisición de usuarios;
- viabilidad técnica;
- viabilidad económica;
- riesgos;
- regulación;
- escalabilidad;
- barreras;
- dependencias externas.

Búsqueda activa de alternativas

Si la propuesta inicial presenta una viabilidad débil o incierta, la IA debe buscar activamente alternativas que puedan mejorarla.

Debe estudiar cuando sea razonable:

- otros públicos;
- otros nichos;
- otros problemas;
- otro posicionamiento;
- otra propuesta de valor;
- B2B;
- B2C;
- B2B2C;
- suscripción;
- pago por uso;
- comisión;
- generación de leads;
- afiliación;
- marketplace;
- publicidad;
- licencias;
- servicio profesional;
- reducción del alcance;
- MVP alternativo;
- automatización parcial;
- integración con servicios existentes;
- pivot parcial;
- pivot completo.

No debe recomendar abandonar una idea simplemente porque su primera formulación sea débil si existe una alternativa razonable que pueda aumentar su viabilidad.

MVP

Determinar cuál es la prueba más pequeña, rápida y económica que permita validar las hipótesis críticas.

Entregable

"estudio-viabilidad.md"

o el entregable específico definido por la plantilla universal correspondiente.

Validación

El estudio debe contener:

- evidencia;
- hipótesis;
- datos;
- fuentes cuando se utilicen;
- análisis;
- alternativas;
- riesgos;
- valoración de viabilidad;
- recomendación.

Debe diferenciarse claramente entre:

- hechos comprobados;
- estimaciones;
- hipótesis;
- opiniones;
- incertidumbres.

Resultado

La IA debe presentar una recomendación:

🟢 CONTINUAR

La oportunidad presenta una viabilidad razonable.

🟠 PIVOTAR

La propuesta original presenta problemas, pero existe una alternativa potencialmente mejor.

🟡 VALIDAR MÁS

La información disponible todavía no permite una conclusión suficientemente sólida.

🔴 NO RECOMENDADO

La evidencia disponible indica una relación riesgo/beneficio desfavorable.

Regla fundamental

La IA informa y recomienda.

La IA NO decide unilateralmente si el proyecto continúa.

La decisión final corresponde al usuario.

El usuario puede decidir:

- continuar;
- continuar con cambios;
- pivotar;
- investigar más;
- detener.

Para avanzar

Debe existir una decisión explícita del usuario cuando el estudio pueda afectar a la decisión de construir.

Si el usuario decide continuar, pasar a Fase 4.

Si decide pivotar y el cambio es sustancial, actualizar el proyecto y repetir el estudio cuando corresponda.

Si decide investigar más, permanecer en esta fase hasta obtener la información necesaria.

Si decide detener, registrar la decisión y cerrar correctamente el proyecto.

Si el estudio no era necesario, esta fase se considera omitida y debe quedar registrado el motivo.

---

FASE 4 — CLASIFICACIÓN

Objetivo

Determinar qué tipo o tipos de proyecto se están construyendo.

Entrada

Fases anteriores validadas y decisión de continuar cuando corresponda.

Acciones

1. Consultar "04-TIPOS-PROYECTO".
2. Comparar el proyecto con los tipos disponibles.
3. Seleccionar el tipo o tipos adecuados.
4. Consultar fixtures relacionados cuando sean útiles.
5. Utilizar los fixtures únicamente como referencia.
6. No copiar datos ficticios al proyecto real.
7. Comprobar que la clasificación sigue siendo coherente con el resultado del estudio previo.

Entregable

Clasificación del proyecto.

Validación

Debe existir una justificación suficiente de la clasificación elegida.

Para avanzar

El tipo de proyecto debe estar identificado o documentarse por qué no encaja en los tipos existentes.

Si falta una categoría reutilizable, registrarla como necesidad antes de continuar.

---

FASE 5 — DEFINICIÓN

Objetivo

Convertir la idea, el análisis y, cuando corresponda, el estudio de viabilidad en una definición concreta y verificable.

Entrada

Fases 1–4 validadas.

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
- validación;
- hipótesis críticas cuando corresponda;
- resultados relevantes del estudio previo cuando corresponda.

ANALYZE

Antes de cerrar la definición, comprobar:

objetivo → alcance → requisitos → criterios de éxito

y comprobar que la definición sigue siendo coherente con:

problema → oportunidad → propuesta → viabilidad.

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

No avanzar si ANALYZE detecta una contradicción crítica.

---

FASE 6 — SELECCIÓN DE MÓDULOS

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

FASE 7 — REQUISITOS

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

FASE 8 — ARQUITECTURA

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

ANALYZE

Comprobar que:

REQUISITOS → ARQUITECTURA

es coherente.

Todo requisito crítico debe tener una solución arquitectónica identificada.

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

No avanzar si ANALYZE detecta incompatibilidades críticas.

---

FASE 9 — PLANIFICACIÓN

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
9. Incorporar las hipótesis críticas del estudio previo cuando corresponda.
10. Incorporar las pruebas necesarias para validar dichas hipótesis.

ANALYZE

Comprobar que:

ARQUITECTURA → PLAN → TAREAS

es ejecutable y no contiene tareas sin propósito.

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

FASE 10 — CONSTRUCCIÓN

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

ANALYZE DURANTE CAMBIOS IMPORTANTES

Cuando durante la construcción aparezca una decisión que pueda afectar:

- objetivo;
- requisitos;
- arquitectura;
- seguridad;
- costes;
- alcance;

se debe ejecutar ANALYZE antes de adoptar el cambio.

Si el cambio modifica el proyecto, debe registrarse en "DECISIONES.md" y actualizar los documentos afectados.

Entregable

Primera versión funcional.

Validación

Cada componente importante debe comprobarse individualmente y dentro del flujo correspondiente.

Para avanzar

Debe existir una versión funcional suficiente para realizar pruebas.

---

FASE 11 — PRUEBAS

Objetivo

Comprobar que el sistema funciona técnicamente y que las hipótesis críticas que requieran prueba pueden ser evaluadas.

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
- regresión;
- hipótesis críticas del proyecto cuando corresponda.

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

FASE 12 — VALIDACIÓN

Objetivo

Determinar si el proyecto resuelve realmente el problema para el que fue creado.

Entrada

Sistema probado.

CONVERGE

Ejecutar CONVERGE.

Comparar:

DEFINICIÓN → REQUISITOS → ARQUITECTURA → IMPLEMENTACIÓN → PRUEBAS

Comprobar también:

REQUISITOS → PRUEBAS → EVIDENCIAS

Y cuando el proyecto tenga hipótesis de negocio:

HIPÓTESIS → EVIDENCIAS → RESULTADO

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
9. criterios de éxito;
10. hipótesis críticas;
11. resultados obtenidos frente a las expectativas iniciales.

Regla

Un sistema técnicamente funcional que no resuelve el problema real no se considera terminado.

Entregable

"validacion.md"

Validación

Debe existir evidencia suficiente de que el sistema cumple el objetivo.

CONVERGE debe producir:

🟢 CONVERGE

o

🟡 AJUSTAR

o

🔴 NO CONVERGE

Para avanzar

Si CONVERGE produce 🟢, el proyecto puede pasar a despliegue.

Si produce 🟡, corregir las diferencias y volver a validar.

Si produce 🔴, identificar la causa y retroceder a la fase correspondiente.

---

FASE 13 — DESPLIEGUE

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

FASE 14 — VALIDACIÓN EN PRODUCCIÓN

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

FASE 15 — MONITORIZACIÓN

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
- cómo


