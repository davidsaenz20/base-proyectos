# PROTOCOLO DE EJECUCIÓN

## 1. OBJETIVO

Este protocolo define cómo debe ejecutarse un proyecto utilizando `base-proyectos`.

Su función es impedir:

- construir demasiado pronto;
- confundir hipótesis con hechos;
- generar URLs sin intención real;
- generar páginas por volumen matemático;
- repetir trabajo existente;
- crear contenido sin demanda validada cuando la demanda sea relevante;
- tomar decisiones importantes sin registrarlas.

El sistema debe trabajar de forma:

- ordenada;
- verificable;
- modular;
- reutilizable;
- escalable;
- orientada a resultados.

# 1.1. CONTINUIDAD Y AMPLIACIÓN DE PROYECTOS EXISTENTES

Un proyecto no termina necesariamente cuando se publica su primera versión.

Una web, sistema o negocio ya construido puede continuar evolucionando mediante:

- nuevas URLs;
- nuevos contenidos;
- nuevas categorías;
- nuevos núcleos temáticos;
- nuevas funcionalidades;
- nuevas formas de monetización;
- nuevas integraciones;
- nuevas automatizaciones;
- mejoras;
- actualizaciones;
- ampliaciones comerciales.

Cuando el usuario indique que está trabajando sobre un proyecto existente, NO se debe reiniciar automáticamente el proceso desde cero.

Primero se debe:

1. identificar el proyecto existente;
2. leer su documentación actual;
3. determinar su estado real;
4. identificar qué partes ya están construidas;
5. identificar qué partes están publicadas;
6. identificar qué se quiere añadir, modificar o ampliar;
7. conservar las decisiones y componentes existentes que sigan siendo válidos;
8. aplicar únicamente las fases necesarias para la nueva actuación;
9. integrar el resultado con lo ya existente.

Ejemplo:

Si una web ya tiene:

- una categoría publicada;
- 10 URLs;
- 10 contenidos;
- WordPress funcionando;
- automatizaciones funcionando;

y el usuario quiere crear una segunda categoría con 10 nuevos contenidos, el sistema debe tratarlo como una AMPLIACIÓN DEL PROYECTO EXISTENTE.

No debe reconstruir:

- la web;
- la categoría existente;
- las URLs existentes;
- los contenidos existentes;
- las automatizaciones existentes;

salvo que la nueva actuación requiera modificarlos.

El mismo principio se aplica si el usuario quiere:

- añadir un nuevo núcleo;
- añadir nuevas URLs a un núcleo existente;
- crear una nueva categoría;
- añadir una tienda de afiliados;
- incorporar una nueva funcionalidad;
- ampliar la monetización;
- crear nuevos contenidos;
- reorganizar una parte de la arquitectura;
- mejorar una sección existente.

El proceso deberá adaptarse al alcance de la actuación.

Por tanto:

PROYECTO NUEVO
↓
PROCESO COMPLETO NECESARIO

PROYECTO EXISTENTE
↓
RECUPERAR ESTADO ACTUAL
↓
IDENTIFICAR ACTUACIÓN
↓
APLICAR SOLO LAS FASES NECESARIAS
↓
INTEGRAR CON LO EXISTENTE
↓
MEDIR
↓
CONTINUAR EVOLUCIONANDO

La existencia de un proyecto publicado no impide volver a utilizar las fases de investigación, demanda, intención, validación, matriz, arquitectura o construcción cuando una nueva actuación lo requiera.

El sistema debe reutilizar el trabajo existente y evitar repetir trabajo innecesariamente.

Una ampliación puede ser pequeña y no requerir todas las fases.

Una ampliación grande puede requerir volver a ejecutar prácticamente todo el proceso para esa nueva parte.

La decisión debe depender del alcance real de la actuación, no de una regla rígida.

---

# 2. PRINCIPIO GENERAL

No construir primero para descubrir después si existe una oportunidad.

Siempre que sea posible:

PROBLEMA

↓

INVESTIGACIÓN

↓

DEMANDA

↓

INTENCIONES

↓

VALIDACIÓN

↓

OPORTUNIDADES

↓

SOLUCIÓN

↓

ARQUITECTURA

↓

CONSTRUCCIÓN

↓

MEDICIÓN

↓

MEJORA

---

# 3. ESTADO DE LA INFORMACIÓN

Toda información relevante debe clasificarse como:

- CONFIRMADO
- PROBABLE
- HIPÓTESIS
- DESCARTADO
- DESCONOCIDO
- PENDIENTE DE VALIDACIÓN

No presentar una hipótesis como un hecho.

No completar información desconocida mediante invención.

---

# 4. PRIMERA FASE: ENTENDER EL PROYECTO

Antes de construir:

1. entender la idea;
2. identificar el objetivo;
3. identificar el usuario;
4. identificar el problema;
5. identificar la solución propuesta;
6. identificar el modelo de negocio;
7. identificar las restricciones;
8. identificar los recursos disponibles;
9. identificar las dependencias;
10. comprobar si existe documentación previa.

Si falta información crítica, detenerse y solicitarla o investigarla.

---

# 5. VALIDAR ANTES DE CONSTRUIR

Determinar qué debe validarse.

Según el proyecto puede ser necesario investigar:

- existencia del problema;
- demanda;
- intención de búsqueda;
- competencia;
- mercado;
- viabilidad económica;
- dificultad técnica;
- posibilidad de automatización;
- capacidad de adquisición;
- monetización;
- riesgos.

No asumir que una idea es viable porque técnicamente puede construirse.

---

# 6. DESCUBRIMIENTO DE DEMANDA E INTENCIONES

Cuando el proyecto dependa de búsquedas de usuarios, utilizar:

`02-MODULOS/DESCUBRIMIENTO-DEMANDA-E-INTENCIONES.md`

La secuencia será:

IDEA / TEMA / SERVICIO

↓

KEYWORDS / CONSULTAS

↓

INTENCIONES

↓

PROBLEMAS Y NECESIDADES

↓

ANÁLISIS DE SERP

↓

AGRUPACIÓN / CLUSTERS

↓

OPORTUNIDADES

↓

TIPOS DE PÁGINA / SOLUCIÓN

↓

ARQUITECTURA

El sistema debe descubrir la demanda antes de generar masivamente URLs.

---

# 7. REGLA KEYWORD → INTENCIÓN → URL

Nunca debe aplicarse:

`1 keyword = 1 URL`

Una keyword es una señal.

Una intención representa una necesidad o resultado que busca el usuario.

Una URL debe existir cuando exista una razón real para que esa página satisfaga una intención diferenciada.

Por tanto:

`KEYWORD ≠ INTENCIÓN ≠ URL`

La cantidad de keywords no determina la cantidad de URLs.

---

# 8. DECIDIR LAS INTENCIONES

Cuando se haya realizado descubrimiento de demanda, determinar:

- intención principal;
- intenciones secundarias;
- problema;
- necesidad;
- resultado esperado;
- etapa del usuario;
- solución esperada;
- oportunidad;
- prioridad.

Las búsquedas deben agruparse por necesidad e intención, no solamente por similitud textual.

---

# 9. MATRIZ DE DECISIÓN DE INTENCIÓN

Antes de convertir las intenciones detectadas en arquitectura o URLs, debe utilizarse:

`02-MODULOS/MATRIZ-DECISION-INTENCION-URL.md`

cuando el proyecto genere, reorganice o priorice páginas a partir de búsquedas.

La matriz debe determinar para cada intención si corresponde:

- CREAR URL;
- AGRUPAR;
- CONVERTIR EN SECCIÓN;
- DESCARTAR;
- MANTENER PENDIENTE DE VALIDACIÓN.

Debe comprobar, cuando corresponda:

- realidad de la intención;
- relación con el proyecto;
- diferenciación respecto a otras intenciones;
- demanda;
- SERP;
- necesidad;
- posibilidad de aportar valor;
- solapamiento;
- potencial comercial;
- necesidad de URL independiente.

La matriz es un mecanismo de decisión.

No es simplemente documentación.

No se debe pasar directamente de keywords a URLs cuando esta fase sea necesaria.

---

# 10. AGRUPACIÓN Y CLUSTERS

Después de analizar las intenciones, agrupar consultas que respondan a la misma necesidad.

Agrupar cuando:

- la necesidad sea esencialmente la misma;
- la respuesta esperada sea equivalente;
- exista un fuerte solapamiento de SERP;
- una misma página pueda resolver adecuadamente las consultas;
- separar las consultas genere páginas redundantes.

Separar cuando:

- cambie la necesidad;
- cambie significativamente la solución;
- cambie la intención;
- la SERP sea diferente;
- exista una intención comercial independiente;
- exista una intención local real;
- una página independiente aporte valor claramente superior.

---

# 11. DECIDIR LAS URLS

A partir de las intenciones validadas y de la matriz de decisión debe determinarse:

- qué URLs crear;
- qué URLs agrupar;
- qué URLs no crear;
- qué páginas serán categorías;
- qué páginas serán contenidos;
- qué páginas serán comerciales;
- qué páginas serán comparativas;
- qué páginas serán locales;
- qué páginas serán herramientas;
- qué páginas serán soluciones integrales.

La arquitectura no debe derivarse automáticamente de una lista de keywords.

Cuando el proyecto dependa de la generación o reorganización de URLs a partir de intenciones de búsqueda, utilizar:

`02-MODULOS/GENERACION-ARQUITECTURA-URLS-POR-INTENCION.md`

Este módulo convierte las decisiones obtenidas en:

- agrupaciones;
- decisiones de páginas;
- tipos de página;
- URLs;
- prioridades;
- arquitectura.

La decisión debe realizarse antes de pasar a la selección definitiva de plantillas y construcción.

---

# 12. REGLA CONTRA LA EXPLOSIÓN DE URLS

No realizar combinaciones cartesianas de variables sin validación.

Ejemplo incorrecto:

`10 servicios × 1.000 localidades × 10 variantes = 100.000 URLs`

La cantidad matemática de combinaciones no demuestra que existan 100.000 intenciones.

Primero:

CONSULTAS

↓

INTENCIONES

↓

CLUSTERS

↓

VALIDACIÓN

↓

DECISIÓN

↓

URLS

Solo las combinaciones justificadas pueden convertirse en páginas.

---

# 13. LOCALIZACIÓN

La combinación:

`SERVICIO + LOCALIDAD`

no debe convertirse automáticamente en una URL.

Antes debe determinarse:

- si existe intención local;
- si la localidad es relevante;
- si existe demanda;
- si existen resultados locales;
- si existe diferenciación;
- si puede aportarse valor;
- si tiene sentido comercial.

La presencia de una localidad en una consulta no demuestra por sí sola que deba existir una landing.

---

# 14. VARIABLES

Las variables detectadas deben analizarse individualmente.

Ejemplos:

- localidad;
- modalidad;
- categoría;
- tamaño;
- presupuesto;
- duración;
- nivel;
- temporada;
- clima;
- tipo de usuario;
- contexto.

Una variable solo debe convertirse en dimensión de URL cuando:

- modifica realmente la intención;
- existe evidencia suficiente;
- aporta valor;
- puede mantenerse;
- no genera una explosión artificial de páginas.

---

# 15. OPORTUNIDADES

Una intención validada no implica automáticamente una página.

Determinar si existe una oportunidad real teniendo en cuenta:

- demanda;
- problema;
- competencia;
- posibilidad de aportar valor;
- monetización;
- dificultad;
- recursos;
- prioridad.

Clasificar las oportunidades como:

- ALTA;
- MEDIA;
- BAJA;
- PENDIENTE.

Registrar las razones de las decisiones importantes.

---

# 16. TIPOS DE PÁGINA

El tipo de página debe derivarse de la intención.

Ejemplos:

`INTENCIÓN INFORMATIVA → GUÍA`

`INTENCIÓN DE PREPARACIÓN → GUÍA / CHECKLIST`

`INTENCIÓN COMPARATIVA → COMPARATIVA`

`INTENCIÓN COMERCIAL → RECOMENDACIÓN / RANKING`

`INTENCIÓN TRANSACCIONAL → PÁGINA COMERCIAL`

`INTENCIÓN LOCAL → LANDING LOCAL`

`INTENCIÓN DE PRODUCTO → REVIEW / FICHA`

`INTENCIÓN COMPLEJA → SOLUCIÓN INTEGRAL`

No asumir que todas las URLs necesitan la misma plantilla.

---

# 17. DISEÑAR LA ARQUITECTURA

La arquitectura debe diseñarse después de disponer de la información necesaria para determinar qué debe existir.

Cuando el proyecto dependa de demanda:

DEMANDA

↓

INTENCIONES

↓

MATRIZ DE DECISIÓN

↓

CLUSTERS

↓

OPORTUNIDADES

↓

TIPOS DE PÁGINA

↓

ARQUITECTURA

↓

URLS

Cuando exista una estructura predeterminada y justificada:

ESTRUCTURA

↓

VALIDACIÓN

↓

ARQUITECTURA

La arquitectura debe representar las necesidades del usuario y la lógica del proyecto.

---

# 18. SELECCIONAR MÓDULOS Y PLANTILLAS

Antes de construir:

1. identificar el tipo de proyecto;
2. consultar `04-TIPOS-PROYECTO/`;
3. identificar módulos necesarios en `02-MODULOS/`;
4. identificar plantillas aplicables en `03-PLANTILLAS/`;
5. comprobar que no exista documentación equivalente;
6. definir dependencias.

Los módulos de demanda, intención y arquitectura deben activarse cuando las condiciones descritas anteriormente lo requieran.

---

# 19. DISEÑO DE PÁGINAS Y PLANTILLAS

Cuando existan diferentes intenciones, no asumir que todas las URLs deben utilizar exactamente la misma estructura.

Determinar:

- tipos de intención;
- tipos de página;
- componentes comunes;
- componentes específicos;
- datos necesarios;
- llamadas a la acción;
- estructura de contenido;
- interlinking.

Ejemplo:

`INTENCIÓN INFORMATIVA → PLANTILLA INFORMATIVA`

`INTENCIÓN COMPARATIVA → PLANTILLA COMPARATIVA`

`INTENCIÓN LOCAL → PLANTILLA LOCAL`

---

# 20. CONSTRUCCIÓN

Construir únicamente después de disponer de:

- problema suficientemente entendido;
- solución definida;
- arquitectura validada;
- decisiones registradas;
- módulos identificados;
- dependencias conocidas.

La construcción debe seguir el orden definido por la arquitectura y las prioridades.

---

# 21. AUTOMATIZACIÓN

La automatización debe utilizarse para reducir trabajo repetitivo, no para sustituir la validación.

Puede automatizar:

- descubrimiento;
- recopilación de consultas;
- clasificación inicial;
- agrupación inicial;
- extracción de datos;
- generación de candidatos;
- generación de estructuras;
- creación de contenidos;
- publicación;
- medición;
- actualización.

Pero las decisiones críticas deben conservar trazabilidad.

---

# 22. GENERACIÓN MASIVA

Antes de generar grandes cantidades de páginas comprobar:

- que la intención esté validada;
- que exista una razón para cada página;
- que no exista duplicación;
- que no exista canibalización;
- que las variables estén justificadas;
- que la plantilla corresponda a la intención;
- que pueda mantenerse la calidad;
- que exista una estrategia de actualización.

Nunca generar miles de páginas únicamente porque el sistema puede hacerlo.

---

# 23. MEDICIÓN

Después de publicar:

- medir resultados;
- comparar con hipótesis;
- detectar páginas sin rendimiento;
- detectar nuevas consultas;
- detectar nuevas intenciones;
- revisar conversiones;
- revisar monetización;
- revisar problemas técnicos;
- revisar oportunidades.

La arquitectura no es necesariamente definitiva.

Los datos reales pueden justificar cambios.

---

# 24. BUCLE DE APRENDIZAJE

El sistema debe funcionar como:

INVESTIGACIÓN

↓

DECISIÓN

↓

CONSTRUCCIÓN

↓

PUBLICACIÓN

↓

DATOS

↓

ANÁLISIS

↓

NUEVAS INTENCIONES

↓

NUEVAS DECISIONES

↓

MEJORA

El proyecto debe aprender de sus propios datos.

---

# 25. DECISIONES

Registrar las decisiones importantes en:

`00-CONTROL/DECISIONES.md`

Una decisión importante debe poder relacionarse con:

- problema;
- evidencia;
- investigación;
- intención;
- oportunidad;
- solución;
- consecuencia.

Cuando la investigación de demanda cambie una hipótesis inicial, debe registrarse el cambio.

---

# 26. DOCUMENTACIÓN

Toda modificación estructural debe reflejarse en la documentación correspondiente.

No crear documentos duplicados si ya existe uno adecuado.

Antes de crear un nuevo archivo:

1. buscar si existe uno equivalente;
2. comprobar su función;
3. determinar si debe modificarse;
4. solo crear uno nuevo si existe una necesidad real.

---

# 27. CONTROL DE CALIDAD

Antes de considerar una fase terminada comprobar:

- ¿la información está validada?
- ¿las hipótesis están identificadas?
- ¿las intenciones están clasificadas?
- ¿la matriz ha sido aplicada cuando corresponde?
- ¿las URLs tienen una razón real?
- ¿se ha evitado la generación artificial de páginas?
- ¿la arquitectura es coherente?
- ¿las decisiones importantes están registradas?
- ¿los archivos están correctamente ubicados?
- ¿las dependencias están resueltas?

Si alguna respuesta crítica es "no", la fase no está terminada.

---

# 28. PRINCIPIO DE TRABAJO

No avanzar por avanzar.

Cada paso debe responder:

1. ¿Qué sabemos?
2. ¿Qué no sabemos?
3. ¿Qué necesitamos validar?
4. ¿Qué decisión debemos tomar?
5. ¿Qué archivo o módulo corresponde?
6. ¿Qué consecuencia tendrá?
7. ¿Cuál es el siguiente paso mínimo útil?

El objetivo no es producir muchos archivos ni muchas páginas.

El objetivo es construir un sistema que permita tomar mejores decisiones y ejecutar proyectos reales de forma reproducible.

---

# 29. REGLA DE ORO

Nunca:

`IDEA → KEYWORDS → URLS → CONTENIDO`

Cuando el proyecto dependa de demanda, utilizar:

`IDEA`

↓

`DEMANDA`

↓

`KEYWORDS / CONSULTAS`

↓

`INTENCIONES`

↓

`PROBLEMAS / NECESIDADES`

↓

`SERP`

↓

`MATRIZ DE DECISIÓN`

↓

`CLUSTERS`

↓

`OPORTUNIDADES`

↓

`TIPOS DE PÁGINA`

↓

`ARQUITECTURA`

↓

`URLS`

↓

`CONTENIDO`

↓

`PUBLICACIÓN`

↓

`MEDICIÓN`

↓

`MEJORA`

La keyword es una señal.

La intención es la unidad de decisión.

La página es una solución.

La URL es la representación técnica de esa solución.
