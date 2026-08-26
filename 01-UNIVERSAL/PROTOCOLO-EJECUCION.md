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

Además, el protocolo incorpora mecanismos transversales de control:

- CLARIFY → aclarar qué se quiere conseguir realmente;
- ANALYZE → comprobar que las decisiones y partes del proyecto son coherentes;
- CONVERGE → comprobar que lo construido coincide con lo definido y que las evidencias demuestran el cumplimiento.

Cuando el proyecto lo requiera, también debe utilizar:

- ESTUDIO PREVIO DE VIABILIDAD → determinar si existe una oportunidad razonable y buscar alternativas para mejorar su viabilidad antes de comprometer recursos importantes.

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

El ROADMAP constituye la referencia para determinar qué trabajo estaba previsto y qué tareas pueden utilizarse para calcular el progreso.

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
- posición de CLARIFY, ANALYZE y CONVERGE dentro del flujo;
- cuándo debe realizarse el estudio previo de viabilidad.

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

1.6 ESTUDIO PREVIO DE VIABILIDAD

"01-UNIVERSAL/ESTUDIO-PREVIO-VIABILIDAD.md"

Define cómo debe analizarse la viabilidad de una propuesta cuando la naturaleza del proyecto lo requiera.

Determina:

- qué aspectos investigar;
- cómo analizar problema, usuario y mercado;
- cómo estudiar competencia;
- cómo analizar alternativas;
- cómo estudiar monetización;
- cómo estudiar costes;
- cómo estudiar viabilidad técnica y económica;
- cómo identificar riesgos;
- cómo buscar pivotes;
- cómo proponer MVP alternativos;
- cómo formular una recomendación;
- cómo separar recomendación del sistema y decisión final del usuario.

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

Cuando el proyecto se encuentre en una fase de estudio previo de viabilidad, también debe consultarse:

"01-UNIVERSAL/ESTUDIO-PREVIO-VIABILIDAD.md"

No es necesario leer toda la documentación del repositorio.

Debe consultarse únicamente la documentación necesaria para el paso actual.

La IA no debe utilizar la memoria de la conversación como sustituto de la documentación persistente cuando la información pueda recuperarse del proyecto.

La memoria conversacional puede servir como apoyo contextual, pero la documentación persistente constituye la fuente de verdad para continuar un proyecto.

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

Toda decisión posterior debe poder relacionarse con el objetivo primario.

Antes de avanzar de una fase a otra, la IA debe comprobar:

¿Lo que estamos haciendo sigue resolviendo el objetivo primario del usuario?

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

CLARIFY no significa preguntar por todo.

La IA debe evitar preguntas innecesarias.

Solo debe preguntar cuando una información pueda cambiar de forma significativa:

- el objetivo;
- el producto;
- el alcance;
- el usuario;
- la arquitectura;
- el resultado final.

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

3.4 GESTIÓN DE APORTACIONES DEL USUARIO

Durante cualquier proyecto el usuario puede aportar:

- nueva información;
- nuevas ideas;
- requisitos;
- ampliaciones;
- correcciones;
- cambios;
- mejoras;
- restricciones;
- decisiones.

Estas aportaciones no deben perderse ni incorporarse silenciosamente.

Flujo obligatorio:

APORTACIÓN

↓

CLASIFICACIÓN

↓

ANÁLISIS

↓

DECISIÓN

↓

REGISTRO

↓

ACTUALIZACIÓN DEL PROYECTO

Toda aportación debe clasificarse como:

- información adicional;
- requisito;
- ampliación;
- mejora;
- idea futura;
- cambio de alcance;
- cambio de objetivo;
- bloqueo;
- decisión.

Una aportación que no cambie sustancialmente el proyecto puede incorporarse al trabajo correspondiente.

Una aportación que pueda modificar:

- objetivo;
- alcance;
- arquitectura;
- costes;
- riesgos;
- resultado esperado;
- funcionamiento final;

debe pasar por ANALYZE antes de modificar el proyecto.

Si cambia sustancialmente el objetivo primario, debe ejecutarse CLARIFY y solicitar confirmación del usuario cuando sea necesario.

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
4. determinar si el paso requiere estudio de viabilidad;
5. ejecutar el trabajo;
6. producir el entregable correspondiente;
7. comprobar el resultado;
8. registrar las decisiones relevantes;
9. ejecutar ANALYZE cuando el trabajo implique decisiones relevantes;
10. registrar cualquier nueva aportación relevante del usuario.

No debe introducir una nueva metodología durante la ejecución sin justificarla.

Ninguna decisión técnica puede sustituir silenciosamente al objetivo del proyecto.

---

5.1 ESTUDIO PREVIO DE VIABILIDAD

Cuando la naturaleza del proyecto requiera comprobar si merece la pena construirlo, la IA debe realizar un estudio previo antes de comprometer recursos importantes en construcción.

Debe utilizar:

"01-UNIVERSAL/ESTUDIO-PREVIO-VIABILIDAD.md"

El estudio debe ser exhaustivo y proporcional al riesgo del proyecto.

Debe investigar, cuando corresponda:

- problema;
- usuario;
- demanda;
- mercado;
- tendencias;
- competencia;
- sustitutos;
- soluciones existentes;
- diferenciación;
- propuesta de valor;
- monetización;
- costes;
- adquisición de usuarios;
- viabilidad técnica;
- viabilidad económica;
- escalabilidad;
- riesgos;
- regulación;
- barreras;
- dependencias externas.

La IA debe buscar activamente alternativas para mejorar la viabilidad cuando la propuesta inicial presente debilidades.

Debe considerar, cuando corresponda:

- cambio de público;
- cambio de nicho;
- cambio de problema;
- cambio de posicionamiento;
- cambio de propuesta de valor;
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
- integración con soluciones existentes;
- pivot parcial;
- pivot completo.

Debe buscar también la forma más pequeña, barata y rápida de validar las hipótesis críticas.

---

5.2 RESULTADO DEL ESTUDIO DE VIABILIDAD

El estudio debe producir una recomendación estructurada.

La IA puede recomendar:

🟢 CONTINUAR

🟠 PIVOTAR

🟡 VALIDAR MÁS

🔴 NO RECOMENDADO

La recomendación debe explicar:

- principales evidencias;
- principales oportunidades;
- principales riesgos;
- incertidumbres;
- alternativas;
- MVP recomendado;
- nivel de confianza.

---

5.3 REGLA FUNDAMENTAL DE DECISIÓN

La IA informa y recomienda.

La IA NO decide unilateralmente el destino del proyecto.

La decisión final corresponde siempre al usuario.

El usuario puede decidir:

- continuar;
- continuar con cambios;
- pivotar;
- investigar más;
- detener.

Una recomendación:

🔴 NO RECOMENDADO

NO equivale automáticamente a:

PROYECTO CANCELADO

La IA debe respetar la decisión del usuario.

Si el usuario decide continuar pese a una recomendación negativa:

1. registrar la decisión;
2. registrar la recomendación del sistema;
3. registrar los riesgos aceptados cuando corresponda;
4. actualizar el estado;
5. continuar con la metodología.

Si el usuario decide pivotar:

1. registrar la decisión;
2. identificar qué cambia;
3. identificar qué permanece;
4. repetir el estudio cuando el cambio sea sustancial;
5. actualizar la documentación.

Si el usuario decide detener:

1. registrar la decisión;
2. conservar el estudio;
3. registrar los motivos;
4. registrar oportunidades futuras;
5. cerrar correctamente el proyecto.

---

5.4 ESTUDIO DE VIABILIDAD Y CONSTRUCCIÓN

No debe iniciarse una construcción técnica significativa cuando el proyecto requiere estudio previo y todavía no existe:

- estudio;
- recomendación;
- decisión del usuario.

Puede realizarse una prueba técnica limitada si dicha prueba es necesaria para determinar la propia viabilidad.

La prueba debe tener un objetivo concreto y no debe convertirse en construcción prematura.

---

5.5 ANALYZE DESPUÉS DEL ESTUDIO

Después del estudio previo, cuando corresponda, ANALYZE debe comprobar:

PROBLEMA → OPORTUNIDAD → PROPUESTA → VIABILIDAD → DECISIÓN → DEFINICIÓN

Debe detectar:

- contradicciones;
- conclusiones no respaldadas;
- hipótesis tratadas como hechos;
- costes omitidos;
- riesgos omitidos;
- alternativas no consideradas cuando sean relevantes;
- decisiones que no coincidan con las evidencias;
- cambios de alcance.

---

6. ANALYZE — CONTROL DE COHERENCIA

ANALYZE debe utilizarse cuando una decisión pueda afectar de forma relevante al proyecto.

Debe comprobar la coherencia entre:

OBJETIVO → PROBLEMA → REQUISITOS → SOLUCIÓN → ARQUITECTURA → PLAN → IMPLEMENTACIÓN

Cuando el proyecto haya pasado por estudio de viabilidad, también debe comprobar:

VIABILIDAD → DECISIÓN → DEFINICIÓN

No es necesario realizar un análisis exhaustivo para cada acción pequeña.

Debe realizarse cuando exista:

- una decisión relevante;
- un cambio;
- una contradicción;
- nueva información;
- una aportación del usuario;
- una desviación potencial;
- una modificación del alcance;
- una conclusión relevante sobre viabilidad.

ANALYZE debe detectar:

- contradicciones;
- requisitos sin solución;
- tareas sin propósito;
- dependencias olvidadas;
- riesgos relevantes;
- decisiones técnicas injustificadas;
- cambios de alcance;
- desviaciones;
- información desconocida que pueda afectar a una decisión crítica;
- inconsistencias entre viabilidad y plan.

Resultado:

🟢 COHERENTE

Se puede continuar.

🟡 DUDAS

Existe información que debe investigarse, verificarse o aclararse.

🔴 CONTRADICCIÓN

Debe corregirse antes de continuar.

---

6.1 REGLA DE ANALYZE

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

6.2 ANALYZE Y CAMBIOS

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

7. VALIDAR

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

7.1 CONVERGE — CONTROL DE IMPLEMENTACIÓN

CONVERGE debe utilizarse para comprobar que el resultado construido corresponde con lo que se había definido.

Debe comparar:

LO DEFINIDO

con:

LO IMPLEMENTADO

y posteriormente:

REQUISITOS → PRUEBAS → EVIDENCIAS

Cuando corresponda, también:

HIPÓTESIS → EVIDENCIAS → RESULTADOS

CONVERGE debe comprobar:

- requisitos cumplidos;
- funcionalidades implementadas;
- diferencias entre diseño e implementación;
- errores;
- decisiones modificadas;
- funcionalidades ausentes;
- funcionalidades innecesarias;
- evidencias insuficientes;
- problemas descubiertos durante las pruebas;
- diferencias entre las hipótesis iniciales y los resultados reales.

Resultado:

🟢 CONVERGE

Lo construido corresponde con lo definido y las evidencias son suficientes.

🟡 AJUSTAR

Existen diferencias menores que deben corregirse.

🔴 NO CONVERGE

La implementación no corresponde suficientemente con el proyecto definido.

No se puede cerrar el proyecto.

---

7.2 CUÁNDO EJECUTAR CONVERGE

CONVERGE debe ejecutarse como mínimo:

1. antes de considerar una solución funcional;
2. después de pruebas relevantes;
3. antes del despliegue cuando el proyecto lo requiera;
4. después de comprobar el funcionamiento real;
5. antes del cierre definitivo del proyecto.

También puede ejecutarse antes si existe una desviación o duda relevante.

---

7.3 CONVERGE NO ES SOLO UNA COMPARACIÓN DE ARCHIVOS

La IA no debe considerar CONVERGE satisfecho simplemente porque:

- los archivos coincidan;
- exista el código;
- las configuraciones estén escritas;
- las pruebas de desarrollo sean correctas.

Debe comprobar que la solución:

resuelve el problema real

y que existe evidencia suficiente.

---

8. ACTUALIZAR EL ESTADO

Cuando un paso termine:

1. validar el resultado;
2. registrar el trabajo realizado;
3. registrar decisiones relevantes;
4. registrar bloqueos si existen;
5. comprobar que el objetivo primario permanece intacto;
6. actualizar "00-CONTROL/ESTADO.md";
7. actualizar las tareas correspondientes cuando proceda;
8. actualizar el progreso únicamente si puede calcularse objetivamente;
9. establecer el siguiente paso únicamente cuando corresponda.

El estado debe reflejar la situación real del proyecto.

---

8.1 PROGRESO OBJETIVO

La IA no debe inventar porcentajes de ejecución.

El progreso general debe proceder del estado real de las tareas registradas en el ROADMAP o en el sistema de tareas del proyecto.

Si todas las tareas tienen el mismo peso:

Progreso = tareas completadas / tareas totales × 100

Si las tareas tienen diferente peso:

Progreso = peso completado / peso total × 100

Reglas:

El porcentaje debe:

1. poder justificarse;
2. proceder del trabajo registrado;
3. corresponder al estado real;
4. poder reconstruirse;
5. actualizarse cuando cambie el estado;
6. no aumentar simplemente porque haya conversación;
7. no aumentar simplemente porque se haya generado documentación;
8. no utilizar estimaciones subjetivas de la IA.

Si no existen suficientes datos:

Progreso general: No calculable

Nunca se debe inventar un porcentaje.

---

9. CONTROL DE DESVIACIONES

Si durante el trabajo aparece una cuestión que no pertenece al paso actual:

Si es necesaria para completar el paso:

Se incorpora al trabajo.

Si es un bloqueo real:

Se detiene el paso y se resuelve el bloqueo.

Si es una mejora, idea o trabajo futuro:

Se registra y se continúa con el paso actual.

Si modifica el objetivo primario:

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

10. BLOQUEOS

Se considera bloqueo aquello que impide completar el paso actual.

Ejemplos:

- falta información crítica;
- dependencia imprescindible no disponible;
- error técnico que impide continuar;
- requisito incompatible;


