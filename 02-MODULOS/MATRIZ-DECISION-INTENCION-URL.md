# MATRIZ DE DECISIÓN: INTENCIÓN → URL

## OBJETIVO

Determinar de forma sistemática cuándo una intención de búsqueda debe:

- generar una URL independiente;
- agruparse con otra intención;
- convertirse en una sección de una página existente;
- descartarse;
- mantenerse pendiente de validación.

Este módulo es reutilizable en cualquier proyecto en el que la arquitectura web deba derivarse de la demanda y de las intenciones de búsqueda.

Puede utilizarse en:

- webs de afiliación;
- webs de contenido;
- webs de servicios;
- directorios;
- marketplaces;
- e-commerce;
- proyectos locales;
- proyectos programáticos;
- otros proyectos con generación o planificación de URLs.

---

# PRINCIPIO FUNDAMENTAL

Una keyword no equivale automáticamente a una URL.

El sistema debe transformar:

KEYWORD / CONSULTA

↓

INTENCIÓN

↓

NECESIDAD

↓

CLUSTER

↓

VALIDACIÓN

↓

DECISIÓN DE PÁGINA

↓

URL

La cantidad de keywords nunca debe determinar por sí sola la cantidad de URLs.

---

# 1. ENTRADA

Para cada consulta descubierta se intentará obtener, cuando sea posible:

- consulta o keyword;
- idioma;
- país;
- mercado;
- intención aparente;
- necesidad que intenta resolver;
- contexto;
- modificadores;
- SERP;
- tipo de resultados predominantes;
- competidores relevantes;
- volumen de búsqueda si existe una fuente fiable;
- tendencia si existe una fuente fiable;
- valor comercial;
- relación con el proyecto;
- posibles consultas equivalentes;
- posibles consultas complementarias.

Los datos desconocidos deben marcarse como desconocidos.

Nunca deben inventarse.

---

# 2. NORMALIZACIÓN

Antes de crear páginas, las consultas deben normalizarse.

Ejemplos de variaciones que pueden representar una misma necesidad:

- qué llevar para senderismo;
- qué llevar a una ruta de senderismo;
- cosas que llevar a una ruta;
- material necesario para senderismo.

No se deben separar automáticamente por diferencias lingüísticas menores.

El sistema debe determinar si las consultas representan realmente necesidades diferentes.

---

# 3. IDENTIFICACIÓN DE INTENCIÓN

Cada consulta debe clasificarse según la intención dominante.

Las categorías disponibles son orientativas y pueden ampliarse cuando el proyecto lo necesite.

## Informativa

El usuario busca aprender, entender o resolver una duda.

Ejemplos:

- cómo hacer X;
- qué es X;
- por qué ocurre X;
- cómo preparar X.

## Preparación

El usuario quiere saber qué necesita para realizar una actividad o alcanzar un objetivo.

Ejemplos:

- qué necesito para acampar;
- qué llevar a una ruta;
- qué material necesito para pescar.

## Comparación

El usuario quiere comparar alternativas.

Ejemplos:

- X vs Y;
- mejor X;
- diferencias entre X e Y.

## Comercial

El usuario está evaluando productos, servicios o soluciones antes de comprar.

Ejemplos:

- mejor mochila de senderismo;
- mejores tiendas de campaña;
- qué mochila comprar.

## Transaccional

El usuario muestra una intención directa de realizar una acción comercial.

Ejemplos:

- comprar X;
- X precio;
- X oferta.

## Local

La necesidad depende de una ubicación concreta.

Ejemplos:

- fontanero Marbella;
- dentista Málaga;
- pesca en determinada localidad.

La existencia de una localidad en la consulta no significa automáticamente que deba existir una URL local.

Debe validarse la intención local.

## Navegacional

El usuario busca una entidad, marca, web o recurso concreto.

## Mixta

Cuando una consulta contiene más de una intención relevante.

En estos casos debe identificarse la intención dominante.

---

# 4. IDENTIFICACIÓN DE NECESIDAD

La keyword es una representación lingüística.

La necesidad es el problema real que el usuario intenta resolver.

Ejemplo:

KEYWORD:

"qué llevar para una ruta de senderismo de un día"

NECESIDAD:

"quiero saber qué necesito para estar preparado durante una ruta de un día."

Otra keyword:

"mejor mochila senderismo 20 litros"

NECESIDAD:

"quiero elegir una mochila adecuada para una ruta de senderismo."

Aunque ambas contienen "senderismo" y "mochila", pueden representar necesidades diferentes.

---

# 5. AGRUPACIÓN DE CONSULTAS

Las consultas deben agruparse cuando:

- responden a la misma necesidad;
- esperan esencialmente la misma respuesta;
- comparten SERP o resultados equivalentes;
- una misma página puede resolverlas completamente;
- separar las consultas provocaría páginas redundantes;
- la diferenciación sería principalmente lingüística.

Ejemplo:

"qué llevar para senderismo"

"qué llevar a una ruta de senderismo"

"material necesario para senderismo"

pueden pertenecer al mismo cluster.

---

# 6. SEPARACIÓN DE INTENCIONES

Las consultas deben separarse cuando:

- la necesidad cambia;
- el usuario espera una respuesta diferente;
- la solución cambia sustancialmente;
- la SERP presenta resultados diferenciados;
- el contexto cambia de forma significativa;
- existe una intención comercial independiente;
- existe una intención local real;
- la página conjunta resultaría demasiado amplia;
- una página independiente puede aportar valor claramente superior.

Ejemplo:

"qué llevar para senderismo"

y

"mejor mochila de senderismo"

no deben fusionarse automáticamente.

La primera responde principalmente a una necesidad de preparación.

La segunda responde principalmente a una necesidad de elección/comparación.

---

# 7. MATRIZ DE DECISIÓN

Cada intención debe pasar por las siguientes preguntas.

| Criterio | Resultado posible |
|---|---|
| ¿La intención es real y comprensible? | Sí / No / Desconocido |
| ¿Está relacionada con el proyecto? | Sí / No |
| ¿Es diferente de otros clusters? | Sí / No / Parcial |
| ¿Existe demanda demostrable? | Sí / No / Desconocido |
| ¿La SERP confirma la intención? | Sí / No / Parcial |
| ¿Existe una necesidad suficientemente concreta? | Sí / No |
| ¿Podemos aportar valor diferencial? | Sí / No / Desconocido |
| ¿Puede resolverse dentro de otra página? | Sí / No |
| ¿Existe potencial comercial? | Sí / No / Desconocido |
| ¿Tiene sentido crear una URL? | Sí / No / Pendiente |

---

# 8. DECISIONES POSIBLES

Después de evaluar una intención solo existen cinco decisiones principales.

## CREAR URL

Utilizar cuando:

- la intención está validada;
- es suficientemente diferenciada;
- necesita una respuesta propia;
- la página aporta valor;
- encaja en la arquitectura.

Resultado:

CREAR URL

---

## AGRUPAR

Utilizar cuando:

- la intención es válida;
- pero puede resolverse mejor dentro de otra página;
- existe solapamiento significativo.

Resultado:

AGRUPAR EN URL EXISTENTE

---

## SECCIÓN

Utilizar cuando:

- la intención merece tratamiento;
- pero no necesita una página independiente;
- puede convertirse en una sección importante de otra página.

Resultado:

SECCIÓN DE URL EXISTENTE

---

## DESCARTAR

Utilizar cuando:

- no existe relación suficiente con el proyecto;
- no hay intención útil;
- la consulta es irrelevante;
- es una duplicación innecesaria;
- no existe posibilidad razonable de aportar valor.

Resultado:

DESCARTAR

---

## PENDIENTE

Utilizar cuando:

- faltan datos;
- la demanda no está validada;
- la SERP es ambigua;
- existe una duda sobre la diferenciación;
- hace falta investigación adicional.

Resultado:

PENDIENTE DE VALIDACIÓN

Nunca convertir una hipótesis en URL definitiva.

---

# 9. VALIDACIÓN DE DEMANDA

Cuando sea posible debe utilizarse información real procedente de herramientas de investigación.

Fuentes posibles:

- Google Keyword Planner;
- Google Trends;
- Search Console cuando el proyecto ya tenga datos;
- herramientas SEO;
- SERP;
- otras fuentes fiables.

El sistema debe diferenciar:

DATOS OBSERVADOS

de

HIPÓTESIS

y de

INFERENCIAS.

Nunca inventar:

- volumen;
- dificultad;
- CPC;
- tendencia;
- tráfico;
- competencia;
- intención.

---

# 10. ANÁLISIS DE SERP

La SERP debe utilizarse para comprobar si Google trata las consultas como una misma necesidad o como necesidades diferentes.

Analizar, cuando sea posible:

- tipo de páginas posicionadas;
- formato predominante;
- intención dominante;
- similitud de resultados;
- entidades presentes;
- características especiales de SERP;
- orientación informativa/comercial/local;
- nivel de especialización.

Si dos consultas muestran esencialmente los mismos resultados y responden a la misma necesidad, existe una señal a favor de agruparlas.

Si muestran resultados claramente diferentes y responden a necesidades diferentes, existe una señal a favor de separarlas.

La SERP es una señal de validación, no una regla absoluta.

---

# 11. CANIBALIZACIÓN

Antes de aprobar una nueva URL debe comprobarse si otra URL existente ya intenta resolver la misma intención.

Si existe una URL equivalente:

- agrupar;
- modificar la URL existente;
- ampliar la página;
- cambiar la orientación;
- o descartar la nueva URL.

No crear dos páginas simplemente porque existen dos keywords diferentes.

---

# 12. LOCALIZACIÓN

La combinación:

SERVICIO + LOCALIDAD

no debe convertirse automáticamente en una URL.

Antes debe determinarse:

- si existe intención local;
- si la localidad es relevante;
- si la demanda es suficiente;
- si existen resultados locales;
- si la página puede ofrecer información o servicios específicos;
- si existe diferenciación real;
- si la combinación tiene sentido comercial.

Esto permite utilizar el mismo sistema tanto para:

"fontanero Marbella"

como para:

"qué llevar para pescar en Marbella"

sin asumir que ambos deben generar URL por el simple hecho de contener una localidad.

---

# 13. VARIABLES

Las variables que aparecen en las consultas deben analizarse individualmente.

Ejemplos:

- localidad;
- modalidad;
- categoría;
- tamaño;
- presupuesto;
- duración;
- nivel de experiencia;
- edad;
- temporada;
- clima;
- tipo de usuario;
- dispositivo;
- contexto.

Una variable solo debe convertirse en dimensión de URL cuando:

- modifica realmente la intención;
- existe demanda o evidencia suficiente;
- aporta valor;
- puede mantenerse;
- no genera una explosión artificial de páginas.

---

# 14. REGLA CONTRA LA EXPLOSIÓN DE URLS

No realizar combinaciones cartesianas de variables sin validación.

Ejemplo incorrecto:

10 servicios × 1.000 localidades × 10 variantes = 100.000 URLs.

La cantidad matemática de combinaciones no demuestra que existan 100.000 intenciones.

Primero debe descubrirse la demanda.

Después:

CONSULTAS

↓

INTENCIONES

↓

CLUSTERS

↓

VALIDACIÓN

↓

URLS

Solo las combinaciones justificadas pueden convertirse en páginas.

---

# 15. MATRIZ KEYWORD → URL

El resultado de cada análisis debe poder registrarse en una tabla como esta:

| Consulta | Intención | Necesidad | Cluster | SERP | Demanda | Acción | URL |
|---|---|---|---|---|---|---|---|
| consulta A | preparación | necesidad A | cluster A | validada | validada | CREAR | /ejemplo/ |
| consulta B | preparación | necesidad A | cluster A | similar | validada | AGRUPAR | /ejemplo/ |
| consulta C | comercial | necesidad B | cluster B | diferente | validada | CREAR | /ejemplo-b/ |
| consulta D | desconocida | necesidad C | cluster C | ambigua | desconocida | PENDIENTE | — |

---

# 16. MATRIZ INTENCIÓN → PÁGINA

Una vez agrupadas las consultas:

| Cluster | Necesidad | Intención dominante | Tipo de página | Acción |
|---|---|---|---|---|
| A | necesidad A | informativa | guía | CREAR |
| B | necesidad B | preparación | checklist | CREAR |
| C | necesidad C | comercial | comparativa | CREAR |
| D | necesidad D | mixta | sección | AGRUPAR |

---

# 17. TIPOS DE PÁGINA

El tipo de página debe derivarse de la intención.

Ejemplos:

| Intención | Página posible |
|---|---|
| Informativa | guía |
| Preparación | guía / checklist |
| Comparativa | comparativa |
| Comercial | ranking / recomendación |
| Transaccional | página comercial |
| Local | landing local / servicio local |
| Producto | ficha / review |
| Mixta | página híbrida |

No utilizar una única plantilla para todas las intenciones.

---

# 18. GENERACIÓN DE URL

La URL debe generarse después de aprobar la intención.

Proceso:

INTENCIÓN VALIDADA

↓

TIPO DE PÁGINA

↓

JERARQUÍA

↓

SLUG

↓

URL

La URL debe:

- ser estable;
- ser legible;
- representar la intención;
- encajar en la arquitectura;
- evitar duplicidades;
- evitar parámetros innecesarios;
- evitar variantes artificiales.

---

# 19. RELACIÓN ENTRE URLS

Una vez aprobadas las URLs debe construirse la relación entre ellas.

Ejemplo:

/senderismo/

/senderismo/que-llevar/

/senderismo/principiantes/

/senderismo/mochila/

/senderismo/mochila/como-elegir/

/senderismo/mochila/mejores/

Cada página debe tener una función clara dentro del conjunto.

---

# 20. PRIORIZACIÓN

No todas las URLs aprobadas tienen que construirse al mismo tiempo.

Priorizar según:

- demanda;
- valor comercial;
- dificultad;
- facilidad de producción;
- autoridad disponible;
- potencial de conversión;
- dependencia respecto a otras páginas;
- coste de creación;
- capacidad de aportar valor diferencial.

La arquitectura completa puede planificarse antes de construirla.

La publicación puede hacerse progresivamente.

---

# 21. AUTOMATIZACIÓN

La automatización puede utilizar este módulo para generar candidatos.

Pero la automatización no debe aprobar automáticamente todas las URLs.

Flujo recomendado:

IDEA

↓

DESCUBRIMIENTO

↓

KEYWORDS / CONSULTAS

↓

NORMALIZACIÓN

↓

INTENCIONES

↓

AGRUPACIÓN

↓

VALIDACIÓN

↓

MATRIZ DE DECISIÓN

↓

URLS APROBADAS

↓

ARQUITECTURA

↓

PLANTILLAS

↓

CONTENIDO

↓

PUBLICACIÓN

↓

MEDICIÓN

↓

REVISIÓN

---

# 22. REGLA PARA PROYECTOS FUTUROS

Cuando un nuevo proyecto necesite generar arquitectura a partir de demanda, este módulo debe ejecutarse antes de la generación masiva de URLs.

El sistema debe comprobar:

1. qué busca realmente el usuario;
2. qué necesidades existen;
3. qué intenciones son diferentes;
4. qué consultas pertenecen a cada intención;
5. qué intenciones pueden agruparse;
6. cuáles necesitan URL propia;
7. cuáles deben convertirse en secciones;
8. cuáles deben descartarse;
9. cuáles requieren más investigación;
10. cómo se transforma cada intención aprobada en una URL.

---

# 23. RESULTADO FINAL ESPERADO

El módulo debe producir como mínimo:

- inventario de consultas;
- clasificación de intenciones;
- agrupación de clusters;
- matriz de decisión;
- decisiones de crear/agrupar/sección/descartar/pendiente;
- tipos de página;
- arquitectura de URLs;
- prioridades de construcción.

El resultado no es una lista de keywords.

El resultado es una **arquitectura web justificada por necesidades e intenciones reales**.

---

# 24. REGLA DE ORO

Nunca:

KEYWORD → URL

Siempre:

KEYWORD

↓

INTENCIÓN

↓

NECESIDAD

↓

CLUSTER

↓

VALIDACIÓN

↓

DECISIÓN

↓

PÁGINA

↓

URL

La keyword es una señal.

La intención es la unidad de decisión.

La URL es el resultado.
