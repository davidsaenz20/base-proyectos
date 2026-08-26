PROTOCOLO DE EJECUCIÓN

PROPÓSITO

Definir cómo debe actuar la IA al iniciar, ejecutar, continuar, validar y reanudar cualquier proyecto utilizando BASE-PROYECTOS.

El objetivo del protocolo es garantizar:

- continuidad;
- trazabilidad;
- no improvisación;
- no desviación;
- fidelidad al objetivo del usuario;
- validación;
- documentación;
- ejecución hasta funcionamiento real.

Además, el protocolo incorpora tres mecanismos transversales de control:

- CLARIFY → aclarar qué se quiere conseguir realmente;
- ANALYZE → comprobar que las decisiones y partes del proyecto son coherentes;
- CONVERGE → comprobar que lo construido coincide con lo definido y que las evidencias demuestran el cumplimiento.

Estos mecanismos no sustituyen las fases del proyecto.

Forman parte del comportamiento obligatorio de la IA durante la ejecución.

---

1. JERARQUÍA DE LA DOCUMENTACIÓN

Durante la ejecución existen diferentes niveles de información.

1.1 ESTADO

"00-CONTROL/ESTADO.md"

Es la fuente única del estado operativo actual.

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

1.2 ROADMAP

"03-PLANTILLAS/ROADMAP.md"

Define el plan específico del proyecto.

Determina:

- qué trabajo debe realizarse;
- tareas;
- orden previsto;
- dependencias;
- criterios específicos de finalización.

No determina el estado actual.

---

1.3 FLUJO DE EJECUCIÓN

"03-PLANTILLAS/FLUJO-EJECUCION-PROYECTO.md"

Define el flujo general de ejecución.

Determina:

- fases generales;
- objetivo de cada fase;
- entradas;
- acciones;
- entregables;
- validaciones;
- condiciones para avanzar;
- posición de CLARIFY, ANALYZE y CONVERGE dentro del flujo.

---

1.4 PLANTILLAS

Las plantillas determinan la estructura de los entregables.

No determinan por sí mismas:

- el estado;
- el siguiente paso;
- el orden global;
- la finalización del proyecto.

---

1.5 DOCUMENTACIÓN UNIVERSAL

La documentación de "01-UNIVERSAL" define reglas, principios y mecanismos reutilizables.

Cuando una regla universal y una decisión específica del proyecto parezcan entrar en conflicto, debe analizarse el conflicto y registrarse la decisión correspondiente.

---

2. RECUPERAR EL CONTEXTO

Antes de comenzar cualquier trabajo se debe revisar, cuando corresponda:

1. "00-CONTROL/ESTADO.md"
2. "03-PLANTILLAS/ROADMAP.md"
3. "03-PLANTILLAS/FLUJO-EJECUCION-PROYECTO.md"
4. decisiones vigentes;
5. bloqueos;
6. documentación relevante;
7. entregables existentes;
8. último progreso registrado.

No es necesario leer toda la documentación del repositorio.

Debe consultarse únicamente la documentación necesaria para el paso actual.

La IA no debe utilizar la memoria de la conversación como sustituto de la documentación persistente cuando la información pueda recuperarse del proyecto.

---

3. IDENTIFICAR EL ESTADO

Antes de ejecutar se debe poder responder:

¿DÓNDE ESTAMOS?

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

3.1 BLOQUEO DEL OBJETIVO PRIMARIO

Antes de iniciar o continuar un proyecto, la IA debe identificar y conservar el objetivo primario expresado por el usuario.

El objetivo primario representa qué quiere conseguir realmente el usuario.

Debe diferenciarse obligatoriamente entre:

- objetivo: qué quiere conseguir el usuario;
- problema: qué necesidad se pretende resolver;
- sistema o producto: qué solución se pretende construir;
- medio técnico: tecnología, plataforma, automatización o herramienta utilizada;
- interfaz: forma mediante la que el usuario interactúa con el sistema;
- mejora o ampliación: funcionalidad adicional que podría incorporarse posteriormente.

Regla fundamental

La IA no puede convertir un medio técnico, una interfaz o una posible implementación en el objetivo principal del proyecto.

Ejemplo

Usuario:

«"Quiero una automatización de reservas para una peluquería."»

Interpretación correcta:

- objetivo: automatizar las reservas;
- problema: gestionar las reservas de forma eficiente;
- sistema: sistema de automatización de reservas;
- medios posibles: n8n, WhatsApp, calendario, formulario, web u otros;
- interfaz: todavía por determinar.

Interpretación incorrecta:

«"Crear una web para una peluquería."»

La web podría formar parte de la solución, pero no puede convertirse en el objetivo principal sin que el usuario lo haya solicitado o confirmado.

Regla de fidelidad

Toda decisión posterior debe poder relacionarse con el objetivo primario.

Antes de avanzar de una fase a otra, la IA debe comprobar:

¿Lo que estamos construyendo sigue resolviendo el objetivo primario del usuario?

Si la respuesta es negativa o dudosa:

1. detener el avance;
2. identificar la desviación;
3. determinar si se trata de una interpretación incorrecta, una mejora o una nueva necesidad;
4. volver al punto correcto del flujo;
5. preguntar al usuario cuando la interpretación no pueda resolverse con la información disponible.

---

3.2 CLARIFY — ACLARAR ANTES DE CONSTRUIR

CLARIFY debe utilizarse obligatoriamente cuando la petición inicial o una decisión posterior pueda interpretarse de varias maneras relevantes.

Su objetivo es evitar construir una solución correcta para un problema que el usuario realmente no pidió.

Debe determinar:

- qué quiere conseguir realmente el usuario;
- qué problema quiere resolver;
- quién utilizará la solución;
- cuál es el resultado esperado;
- qué está dentro del alcance;
- qué está fuera del alcance;
- qué información crítica falta;
- qué supuestos no deben realizarse.

CLARIFY no significa preguntar por todo

La IA debe evitar preguntas innecesarias.

Solo debe preguntar cuando una información pueda cambiar de forma significativa:

- el objetivo;
- el producto;
- el alcance;
- el usuario;
- la arquitectura;
- el resultado final.

Regla

Si la ambigüedad no cambia materialmente el proyecto, la IA puede continuar.

Si puede cambiar materialmente el proyecto, debe aclararse antes de continuar.

---

3.3 REGISTRO DE CLARIFY

La salida de CLARIFY debe quedar reflejada en el proyecto cuando sea relevante para futuras decisiones.

Como mínimo debe quedar determinado:

OBJETIVO

PROBLEMA

USUARIO

RESULTADO ESPERADO

ALCANCE

FUERA DE ALCANCE

DUDAS CRÍTICAS

No es obligatorio crear un documento adicional para cada CLARIFY.

Debe utilizarse la documentación del proyecto que corresponda.

---

4. IDENTIFICAR EL PASO ACTUAL

Debe existir una única acción principal en curso.

La IA debe trabajar sobre ese paso antes de iniciar otro.

No debe ejecutar simultáneamente varias líneas de trabajo independientes salvo que sean necesarias para completar el mismo paso.

---

5. EJECUTAR

Realizar únicamente el trabajo necesario para completar el paso actual.

La IA debe:

1. consultar la documentación necesaria;
2. comprobar el objetivo primario cuando el trabajo pueda afectar al alcance;
3. ejecutar CLARIFY cuando exista una ambigüedad crítica;
4. ejecutar el trabajo;
5. producir el entregable correspondiente;
6. comprobar el resultado;
7. registrar las decisiones relevantes;
8. ejecutar ANALYZE cuando el trabajo implique decisiones relevantes.

No debe introducir una nueva metodología durante la ejecución sin justificarla.

Ninguna decisión técnica puede sustituir silenciosamente al objetivo del proyecto.

---

5.1 ANALYZE — CONTROL DE COHERENCIA

ANALYZE debe utilizarse cuando una decisión pueda afectar de forma relevante al proyecto.

Debe comprobar la coherencia entre:

OBJETIVO → PROBLEMA → REQUISITOS → SOLUCIÓN → ARQUITECTURA → PLAN → IMPLEMENTACIÓN

No es necesario realizar un análisis exhaustivo para cada acción pequeña.

Debe realizarse cuando exista una decisión relevante, un cambio, una contradicción, una nueva información o una desviación potencial.

ANALYZE debe detectar

- contradicciones;
- requisitos sin solución;
- tareas sin propósito;
- dependencias olvidadas;
- riesgos relevantes;
- decisiones técnicas injustificadas;
- cambios de alcance;
- desviaciones;
- información desconocida que pueda afectar a una decisión crítica.

Resultado

ANALYZE debe producir internamente uno de estos estados:

🟢 COHERENTE

Se puede continuar.

🟡 DUDAS

Existe información que debe investigarse, verificarse o aclararse.

🔴 CONTRADICCIÓN

Debe corregirse antes de continuar.

---

5.2 REGLA DE ANALYZE

Si ANALYZE detecta una contradicción crítica:

NO SE DEBE CONTINUAR CONSTRUYENDO SOBRE ESA CONTRADICCIÓN.

La IA debe:

1. detener el paso afectado;
2. identificar la contradicción;
3. explicar su impacto;
4. determinar si puede resolverse con documentación existente;
5. investigar si procede;
6. preguntar al usuario si es necesario;
7. registrar la decisión;
8. actualizar los documentos afectados;
9. continuar únicamente después de resolverla.

---

5.3 ANALYZE Y CAMBIOS

Cuando durante la construcción aparezca una decisión que pueda afectar:

- objetivo;
- requisitos;
- arquitectura;
- seguridad;
- costes;
- alcance;
- integraciones;
- funcionamiento real;

se debe ejecutar ANALYZE antes de adoptar el cambio.

Si el cambio modifica el proyecto, debe registrarse en "DECISIONES.md" y actualizar los documentos afectados.

---

6. VALIDAR

Todo paso debe tener una validación.

No se considera terminado un paso simplemente porque:

- se haya creado un archivo;
- se haya escrito documentación;
- se haya realizado una configuración;
- se haya ejecutado una acción.

Debe comprobarse que el resultado cumple su criterio de salida.

Además, cuando corresponda, debe comprobarse que el resultado sigue siendo coherente con el objetivo primario del proyecto.

La validación de un paso no implica automáticamente que el proyecto completo esté terminado.

---

6.1 CONVERGE — CONTROL DE IMPLEMENTACIÓN

CONVERGE debe utilizarse para comprobar que el resultado construido corresponde con lo que se había definido.

Debe comparar:

LO DEFINIDO

con:

LO IMPLEMENTADO

y posteriormente:

REQUISITOS → PRUEBAS → EVIDENCIAS

CONVERGE debe comprobar

- requisitos cumplidos;
- funcionalidades implementadas;
- diferencias entre diseño e implementación;
- errores;
- decisiones modificadas;
- funcionalidades ausentes;
- funcionalidades innecesarias;
- evidencias insuficientes;
- problemas descubiertos durante las pruebas.

Resultado

🟢 CONVERGE

Lo construido corresponde con lo definido y las evidencias son suficientes.

🟡 AJUSTAR

Existen diferencias menores que deben corregirse.

🔴 NO CONVERGE

La implementación no corresponde suficientemente con el proyecto definido.

No se puede cerrar el proyecto.

---

6.2 CUÁNDO EJECUTAR CONVERGE

CONVERGE debe ejecutarse como mínimo:

1. antes de considerar una solución funcional;
2. después de pruebas relevantes;
3. antes del despliegue cuando el proyecto lo requiera;
4. después de comprobar el funcionamiento real;
5. antes del cierre definitivo del proyecto.

También puede ejecutarse antes si existe una desviación o duda relevante.

---

6.3 CONVERGE NO ES SOLO UNA COMPARACIÓN DE ARCHIVOS

La IA no debe considerar CONVERGE satisfecho simplemente porque:

- los archivos coincidan;
- exista el código;
- las configuraciones estén escritas;
- las pruebas de desarrollo sean correctas.

Debe comprobar que la solución:

resuelve el problema real

y que existe evidencia suficiente.

---

7. ACTUALIZAR EL ESTADO

Cuando un paso termine:

1. validar el resultado;
2. registrar el trabajo realizado;
3. registrar decisiones relevantes;
4. registrar bloqueos si existen;
5. comprobar que el objetivo primario permanece intacto;
6. actualizar "00-CONTROL/ESTADO.md";
7. establecer el siguiente paso únicamente cuando corresponda.

El estado debe reflejar la situación real del proyecto.

---

8. CONTROL DE DESVIACIONES

Si durante el trabajo aparece una cuestión que no pertenece al paso actual:

Si es necesaria para completar el paso

Se incorpora al trabajo.

Si es un bloqueo real

Se detiene el paso y se resuelve el bloqueo.

Si es una mejora, idea o trabajo futuro

Se registra y se continúa con el paso actual.

Si modifica el objetivo primario

No se incorpora automáticamente.

Debe:

1. identificar el cambio;
2. ejecutar CLARIFY;
3. explicar por qué afecta al objetivo;
4. distinguirlo del objetivo original;
5. ejecutar ANALYZE;
6. solicitar confirmación del usuario cuando corresponda;
7. registrar la decisión;
8. actualizar la documentación si el usuario confirma el cambio.

No se debe cambiar automáticamente de objetivo.

---

9. BLOQUEOS

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

10. CAMBIOS DE PLAN

El roadmap puede cambiar cuando exista una razón real.

Si es necesario modificarlo:

1. explicar el motivo;
2. ejecutar ANALYZE;
3. registrar la decisión;
4. actualizar el roadmap;
5. actualizar "ESTADO.md";
6. comprobar que el objetivo primario continúa siendo el mismo o registrar formalmente su modificación;
7. continuar desde el nuevo paso.

No se debe cambiar el plan simplemente porque aparezca una idea mejor.

---

11. REGLA DE NO RETROCESO

No se debe retroceder de fase por iniciativa propia.

Solo se retrocede cuando:

- una validación demuestra un problema;
- existe un bloqueo;
- una decisión anterior impide continuar;
- aparece información nueva que invalida una decisión crítica;
- se detecta una desviación respecto al objetivo primario;
- CONVERGE determina que lo construido no corresponde con lo definido.

Cuando se retrocede:

1. documentar la causa;
2. identificar la fase afectada;
3. actualizar ESTADO;
4. resolver;
5. volver al flujo normal.

---

12. REGLA PARA "SIGUE"

Cuando el usuario indique:

"Sigue"

la IA debe interpretar la orden como:

«Continuar el proyecto desde el estado persistente actual.»

Debe:

1. recuperar "ESTADO.md";
2. identificar fase y paso actuales;
3. comprobar qué está hecho;
4. identificar qué falta;
5. comprobar el objetivo primario;
6. ejecutar CLARIFY si existe una ambigüedad crítica;
7. ejecutar ANALYZE si existe una decisión, contradicción o cambio relevante;
8. consultar la documentación necesaria;
9. ejecutar el trabajo correspondiente;
10. validar;
11. ejecutar CONVERGE cuando corresponda;
12. actualizar el estado;
13. continuar únicamente si el criterio de avance está cumplido.

"Sigue" no significa:

- cambiar de fase;
- empezar una idea nueva;
- cambiar el objetivo;
- crear una nueva metodología;
- investigar algo no relacionado;
- rehacer trabajo ya validado.

---

13. REGLA DE CONTINUIDAD

La conversación puede interrumpirse en cualquier momento.

Cuando el proyecto se reanude, la IA debe poder continuar utilizando la documentación persistente.

No debe depender de recordar conversaciones anteriores.

Debe poder responder:

DÓNDE ESTAMOS → QUÉ ESTÁ HECHO → QUÉ FALTA → QUÉ TOCA AHORA → CUÁL ES EL OBJETIVO PRIMARIO

Y, cuando corresponda:

QUÉ SE HA DECIDIDO → QUÉ SE HA VALIDADO → QUÉ NO CONVERGE

---

14. REGLA DE NO IMPROVISACIÓN

Si existe información crítica desconocida:

- no inventarla;
- no asumirla como cierta;
- no construir sobre ella.

Determinar si:

1. puede investigarse;
2. puede verificarse;
3. debe preguntarse al usuario;
4. puede posponerse sin bloquear.

Cuando la información desconocida pueda cambiar sustancialmente la interpretación del proyecto, debe ejecutarse CLARIFY y preguntarse antes de avanzar cuando sea necesario.

Cuando la información pueda afectar una decisión técnica relevante, debe ejecutarse ANALYZE.

---

15. REGLA DE DOCUMENTACIÓN

Toda información necesaria para continuar el proyecto debe quedar registrada en la documentación correspondiente.

La conversación no debe ser necesaria para reconstruir el estado del proyecto.

Las decisiones importantes deben conservarse.

El objetivo primario debe poder reconstruirse desde la documentación persistente.

Los resultados relevantes de CLARIFY, ANALYZE y CONVERGE deben quedar documentados cuando afecten a decisiones, cambios o validaciones importantes.

No es obligatorio registrar cada comprobación trivial.

---

16. REGLA DE VALIDACIÓN REAL

El objetivo final no es producir documentación.

El objetivo final es construir una solución que funcione realmente.

Por tanto:

documentado ≠ terminado

implementado ≠ validado

probado en desarrollo ≠ funcionando en producción

Un proyecto solo puede considerarse terminado cuando:

- el flujo real haya sido comprobado;
- los criterios de cierre se hayan cumplido;
- CONVERGE final sea satisfactorio.

---

17. REANUDACIÓN

Cuando se retome un proyecto después de una interrupción:

1. leer ESTADO;
2. leer el roadmap cuando sea necesario;
3. identificar la fase;
4. identificar el paso;
5. comprobar el objetivo primario;
6. comprobar el entregable pendiente;
7. comprobar bloqueos;
8. revisar las decisiones relevantes;
9. comprobar si existe alguna desviación;
10. ejecutar CLARIFY si existe una ambigüedad crítica;
11. ejecutar ANALYZE si existe una contradicción o decisión relevante;
12. continuar.

No comenzar desde la memoria de la conversación.

---

18. REGLA FINAL

La IA debe trabajar siempre con esta secuencia:

RECUPERAR → CLARIFY → IDENTIFICAR → ANALYZE → EJECUTAR → VALIDAR → CONVERGE → DOCUMENTAR → ACTUALIZAR → AVANZAR

No todos los mecanismos requieren una ejecución completa en cada acción.

Pero deben ejecutarse obligatoriamente cuando el contexto lo requiera según las reglas anteriores.

Y siempre respetando:

ESTADO = dónde estamos

ROADMAP = qué trabajo está planificado

FLUJO = cómo se ejecuta

PLANTILLAS = cómo se estructuran los entregables

PROTOCOLO = cómo debe comportarse la IA

OBJETIVO PRIMARIO = qué quiere conseguir realmente el usuario

CLARIFY = qué quiere decir realmente el usuario

ANALYZE = si las partes del proyecto son coherentes

CONVERGE = si lo construido corresponde con lo definido y funciona realmente

---

PRINCIPIO PRINCIPAL

La IA no debe limitarse a ayudar a documentar un proyecto.

Debe guiarlo desde:

IDEA

hasta:

SISTEMA FUNCIONANDO EN LA REALIDAD

sin perder el contexto, sin improvisar y sin desviarse innecesariamente.

Y, sobre todo:

NO DEBE CONFUNDIR EL OBJETIVO DEL USUARIO CON EL MEDIO UTILIZADO PARA CONSEGUIRLO.

NO DEBE CONSTRUIR UNA SOLUCIÓN ANTES DE HABER ENTENDIDO QUÉ SE QUIERE CONSEGUIR.

NO DEBE SEGUIR CONSTRUYENDO CUANDO EXISTE UNA CONTRADICCIÓN CRÍTICA.

NO DEBE CONSIDERAR TERMINADO LO QUE NO CONVERGE CON EL OBJETIVO, LOS REQUISITOS Y LAS EVIDENCIAS.



