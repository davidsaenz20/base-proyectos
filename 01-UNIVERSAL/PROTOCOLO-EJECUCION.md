# PROTOCOLO DE EJECUCIÓN

## PROPÓSITO

Definir cómo debe actuar la IA al iniciar, ejecutar, continuar, validar y reanudar cualquier proyecto utilizando BASE-PROYECTOS.

El objetivo del protocolo es garantizar:

- continuidad;
- trazabilidad;
- no improvisación;
- no desviación;
- validación;
- documentación;
- ejecución hasta funcionamiento real.

---

# 1. JERARQUÍA DE LA DOCUMENTACIÓN

Durante la ejecución existen diferentes niveles de información.

## 1.1 ESTADO

`00-CONTROL/ESTADO.md`

Es la fuente única del **estado operativo actual**.

Determina:

- fase actual;
- paso actual;
- estado;
- progreso;
- bloqueos;
- decisiones relevantes;
- validaciones;
- siguiente acción.

Ningún otro documento debe competir con ESTADO para indicar dónde se encuentra actualmente el proyecto.

---

## 1.2 ROADMAP

`03-PLANTILLAS/ROADMAP.md`

Define el **plan específico del proyecto**.

Determina:

- qué trabajo debe realizarse;
- tareas;
- orden previsto;
- dependencias;
- criterios específicos de finalización.

No determina el estado actual.

---

## 1.3 FLUJO DE EJECUCIÓN

`03-PLANTILLAS/FLUJO-EJECUCION-PROYECTO.md`

Define el **flujo general de ejecución**.

Determina:

- fases generales;
- objetivo de cada fase;
- entradas;
- acciones;
- entregables;
- validaciones;
- condiciones para avanzar.

---

## 1.4 PLANTILLAS

Las plantillas determinan la estructura de los entregables.

No determinan por sí mismas:

- el estado;
- el siguiente paso;
- el orden global;
- la finalización del proyecto.

---

## 1.5 DOCUMENTACIÓN UNIVERSAL

La documentación de `01-UNIVERSAL` define reglas, principios y mecanismos reutilizables.

---

# 2. RECUPERAR EL CONTEXTO

Antes de comenzar cualquier trabajo se debe revisar, cuando corresponda:

1. `00-CONTROL/ESTADO.md`
2. `03-PLANTILLAS/ROADMAP.md`
3. `03-PLANTILLAS/FLUJO-EJECUCION-PROYECTO.md`
4. decisiones vigentes;
5. bloqueos;
6. documentación relevante;
7. entregables existentes;
8. último progreso registrado.

No es necesario leer toda la documentación del repositorio.

Debe consultarse únicamente la documentación necesaria para el paso actual.

---

# 3. IDENTIFICAR EL ESTADO

Antes de ejecutar se debe poder responder:

**¿DÓNDE ESTAMOS?**

Debe existir:

- proyecto identificado;
- fase actual;
- paso actual;
- objetivo del paso;
- entregable esperado;
- criterio de validación.

Si alguno de estos elementos críticos no puede determinarse, no se debe improvisar.

Debe recuperarse la información necesaria o preguntar al usuario si realmente falta información.

---

# 4. IDENTIFICAR EL PASO ACTUAL

Debe existir **una única acción principal en curso**.

La IA debe trabajar sobre ese paso antes de iniciar otro.

No debe ejecutar simultáneamente varias líneas de trabajo independientes salvo que sean necesarias para completar el mismo paso.

---

# 5. EJECUTAR

Realizar únicamente el trabajo necesario para completar el paso actual.

La IA debe:

1. consultar la documentación necesaria;
2. ejecutar;
3. producir el entregable correspondiente;
4. comprobar el resultado;
5. registrar las decisiones relevantes.

No debe introducir una nueva metodología durante la ejecución sin justificarla.

---

# 6. VALIDAR

Todo paso debe tener una validación.

No se considera terminado un paso simplemente porque:

- se haya creado un archivo;
- se haya escrito documentación;
- se haya realizado una configuración;
- se haya ejecutado una acción.

Debe comprobarse que el resultado cumple su criterio de salida.

---

# 7. ACTUALIZAR EL ESTADO

Cuando un paso termine:

1. validar el resultado;
2. registrar el trabajo realizado;
3. registrar decisiones relevantes;
4. registrar bloqueos si existen;
5. actualizar `00-CONTROL/ESTADO.md`;
6. establecer el siguiente paso únicamente cuando corresponda.

El estado debe reflejar la situación real del proyecto.

---

# 8. CONTROL DE DESVIACIONES

Si durante el trabajo aparece una cuestión que no pertenece al paso actual:

### Si es necesaria para completar el paso

Se incorpora al trabajo.

### Si es un bloqueo real

Se detiene el paso y se resuelve el bloqueo.

### Si es una mejora, idea o trabajo futuro

Se registra y se continúa con el paso actual.

No se debe cambiar automáticamente de objetivo.

---

# 9. BLOQUEOS

Se considera bloqueo aquello que impide completar el paso actual.

Ejemplos:

- falta información crítica;
- dependencia imprescindible no disponible;
- error técnico que impide continuar;
- requisito incompatible;
- decisión necesaria que no puede tomarse con la información disponible.

No son bloqueos por sí mismos:

- mejoras;
- optimizaciones;
- ideas nuevas;
- alternativas;
- refactorizaciones;
- documentación no necesaria para el paso actual.

Si existe un bloqueo:

1. identificarlo;
2. documentarlo;
3. determinar qué falta;
4. resolverlo;
5. validar;
6. continuar.

---

# 10. CAMBIOS DE PLAN

El roadmap puede cambiar cuando exista una razón real.

Si es necesario modificarlo:

1. explicar el motivo;
2. registrar la decisión;
3. actualizar el roadmap;
4. actualizar `ESTADO.md`;
5. continuar desde el nuevo paso.

No se debe cambiar el plan simplemente porque aparezca una idea mejor.

---

# 11. REGLA DE NO RETROCESO

No se debe retroceder de fase por iniciativa propia.

Solo se retrocede cuando:

- una validación demuestra un problema;
- existe un bloqueo;
- una decisión anterior impide continuar;
- aparece información nueva que invalida una decisión crítica.

Cuando se retrocede:

1. documentar la causa;
2. identificar la fase afectada;
3. actualizar ESTADO;
4. resolver;
5. volver al flujo normal.

---

# 12. REGLA PARA "SIGUE"

Cuando el usuario indique:

**"Sigue"**

la IA debe interpretar la orden como:

> Continuar el proyecto desde el estado persistente actual.

Debe:

1. recuperar `ESTADO.md`;
2. identificar fase y paso actuales;
3. comprobar qué está hecho;
4. identificar qué falta;
5. consultar la documentación necesaria;
6. ejecutar el trabajo correspondiente;
7. validar;
8. actualizar el estado;
9. continuar únicamente si el criterio de avance está cumplido.

**"Sigue" no significa:**

- cambiar de fase;
- empezar una idea nueva;
- crear una nueva metodología;
- investigar algo no relacionado;
- rehacer trabajo ya validado.

---

# 13. REGLA DE CONTINUIDAD

La conversación puede interrumpirse en cualquier momento.

Cuando el proyecto se reanude, la IA debe poder continuar utilizando la documentación persistente.

No debe depender de recordar conversaciones anteriores.

Debe poder responder:

**DÓNDE ESTAMOS → QUÉ ESTÁ HECHO → QUÉ FALTA → QUÉ TOCA AHORA**

---

# 14. REGLA DE NO IMPROVISACIÓN

Si existe información crítica desconocida:

- no inventarla;
- no asumirla como cierta;
- no construir sobre ella.

Determinar si:

1. puede investigarse;
2. puede verificarse;
3. debe preguntarse al usuario;
4. puede posponerse sin bloquear.

---

# 15. REGLA DE DOCUMENTACIÓN

Toda información necesaria para continuar el proyecto debe quedar registrada en la documentación correspondiente.

La conversación no debe ser necesaria para reconstruir el estado del proyecto.

Las decisiones importantes deben conservarse.

---

# 16. REGLA DE VALIDACIÓN REAL

El objetivo final no es producir documentación.

El objetivo final es construir una solución que funcione realmente.

Por tanto:

**documentado ≠ terminado**

**implementado ≠ validado**

**probado en desarrollo ≠ funcionando en producción**

Un proyecto solo puede considerarse terminado cuando el flujo real haya sido comprobado y los criterios de cierre se hayan cumplido.

---

# 17. REANUDACIÓN

Cuando se retome un proyecto después de una interrupción:

1. leer ESTADO;
2. leer el roadmap cuando sea necesario;
3. identificar la fase;
4. identificar el paso;
5. comprobar el entregable pendiente;
6. comprobar bloqueos;
7. revisar las decisiones relevantes;
8. continuar.

No comenzar desde la memoria de la conversación.

---

# 18. REGLA FINAL

La IA debe trabajar siempre con esta secuencia:

**RECUPERAR → IDENTIFICAR → EJECUTAR → VALIDAR → DOCUMENTAR → ACTUALIZAR → AVANZAR**

Y siempre respetando:

**ESTADO = dónde estamos**

**ROADMAP = qué trabajo está planificado**

**FLUJO = cómo se ejecuta**

**PLANTILLAS = cómo se estructuran los entregables**

**PROTOCOLO = cómo debe comportarse la IA**

---

# PRINCIPIO PRINCIPAL

La IA no debe limitarse a ayudar a documentar un proyecto.

Debe guiarlo desde:

**IDEA**

hasta:

**SISTEMA FUNCIONANDO EN LA REALIDAD**

sin perder el contexto, sin improvisar y sin desviarse innecesariamente.


