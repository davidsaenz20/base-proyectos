# MÓDULO UNIVERSAL DE GENERACIÓN DE ARQUITECTURA DE URLS POR INTENCIÓN

## PROPÓSITO

Convertir el resultado del descubrimiento de demanda e intenciones en una arquitectura de páginas y URLs coherente, priorizada y justificable.

Este módulo funciona después de:

`DESCUBRIMIENTO DE DEMANDA E INTENCIONES`

y antes de:

`ARQUITECTURA → PLANTILLAS → CONSTRUCCIÓN`

No genera URLs simplemente a partir de keywords.

Su función es determinar qué intenciones necesitan una página independiente, qué intenciones deben agruparse, qué páginas deben descartarse y qué estructura de URLs debe construirse.

---

# 1. PRINCIPIO FUNDAMENTAL

KEYWORD ≠ INTENCIÓN ≠ URL

El sistema nunca debe aplicar:

`1 keyword = 1 URL`

Debe aplicar:

`KEYWORDS → INTENCIONES → OPORTUNIDADES → PÁGINAS → URLS`

Una URL solamente debe existir cuando exista una razón funcional, informativa, comercial o estructural para crearla.

---

# 2. ENTRADA

Este módulo recibe, cuando estén disponibles:

- idea del proyecto;
- modelo de negocio;
- público objetivo;
- territorio;
- idioma;
- keywords;
- consultas;
- intenciones;
- clusters;
- problemas;
- necesidades;
- oportunidades;
- datos de demanda;
- análisis de SERP;
- competencia;
- monetización;
- tipos de página disponibles;
- restricciones del proyecto.

También puede recibir una estructura de URLs previamente definida.

---

# 3. DOS MODOS DE FUNCIONAMIENTO

## MODO A — ARQUITECTURA DESCUBIERTA

Se utiliza cuando las URLs todavía no están definidas.

Proceso:

`IDEA`

↓

`DEMANDA`

↓

`KEYWORDS`

↓

`INTENCIONES`

↓

`CLUSTERS`

↓

`OPORTUNIDADES`

↓

`TIPOS DE PÁGINA`

↓

`URLS`

↓

`ARQUITECTURA`

---

## MODO B — ARQUITECTURA PREDEFINIDA

Se utiliza cuando existe una lógica externa suficientemente justificada.

Ejemplo:

`SERVICIO + LOCALIDAD`

En este caso no es necesario descubrir cada URL desde cero.

El sistema debe:

1. recibir la matriz;
2. comprobar su coherencia;
3. validar las combinaciones;
4. detectar excepciones;
5. detectar oportunidades adicionales;
6. detectar duplicidades;
7. priorizar;
8. generar la arquitectura final.

La investigación de demanda se utilizará para mejorar la estructura cuando aporte valor.

---

# 4. IDENTIFICACIÓN DE INTENCIONES

Cada oportunidad debe contener como mínimo:

- identificador;
- intención;
- problema;
- necesidad;
- keywords asociadas;
- tipo de usuario;
- etapa del usuario;
- tipo de solución;
- potencial de monetización;
- prioridad;
- URL propuesta;
- justificación.

---

# 5. DECISIÓN DE PÁGINA

Para cada intención el sistema debe decidir:

### A — PÁGINA INDEPENDIENTE

Cuando la intención representa una necesidad diferenciada.

### B — AGRUPAR

Cuando varias intenciones pueden resolverse correctamente mediante una misma página.

### C — INCLUIR COMO SECCIÓN

Cuando la necesidad es relevante pero no necesita una página propia.

### D — DESCARTAR

Cuando no existe suficiente valor o justificación.

---

# 6. REGLA DE AGRUPACIÓN

Antes de crear una nueva URL debe realizarse esta pregunta:

> ¿Puede una única página satisfacer correctamente esta intención y las intenciones relacionadas?

Si la respuesta es sí:

`AGRUPAR`

Si la respuesta es no:

`SEPARAR`

La decisión debe considerar:

- objetivo del usuario;
- necesidad;
- solución;
- contenido requerido;
- SERP;
- tipo de página;
- intención comercial;
- posibilidad de satisfacer la búsqueda;
- riesgo de canibalización.

---

# 7. VALIDACIÓN DE SERP

Cuando sea posible, comparar las consultas candidatas.

Si dos consultas muestran resultados sustancialmente equivalentes y buscan la misma solución:

`POSIBLE MISMA URL`

Si muestran resultados claramente diferentes y requieren soluciones diferentes:

`POSIBLES URLS DIFERENTES`

La SERP es una señal para tomar la decisión, no una regla matemática absoluta.

---

# 8. DETECCIÓN DE DUPLICIDADES

Antes de aprobar una URL, comprobar:

- misma intención;
- mismo problema;
- misma solución;
- misma audiencia;
- mismo tipo de página;
- contenido prácticamente equivalente;
- variaciones lingüísticas;
- sinónimos;
- cambios mínimos de palabras;
- variantes artificiales.

Si la única diferencia es una variante lingüística o textual sin necesidad diferenciada:

`NO CREAR NUEVA URL`

---

# 9. CANIBALIZACIÓN

Cada nueva URL debe compararse con las existentes.

Debe detectarse si:

- responde a la misma intención;
- compite por las mismas consultas;
- requiere prácticamente el mismo contenido;
- puede fusionarse;
- puede convertirse en una sección;
- necesita una diferenciación explícita.

Resultado:

`MANTENER`

`FUSIONAR`

`REDIRIGIR`

`DIFERENCIAR`

`DESCARTAR`

---

# 10. TIPO DE PÁGINA

La intención debe determinar el tipo de página más adecuado.

Ejemplos:

| Intención | Tipo de página |
|---|---|
| Qué necesito para... | Guía/checklist |
| Cómo hacer... | Tutorial |
| Mejor X | Comparativa |
| X vs Y | Comparativa |
| Alternativas a X | Alternativas |
| Comprar X | Comercial |
| Precio de X | Comercial/informativa |
| X en localidad | Landing local |
| Servicio X | Página de servicio |
| Categoría de productos | Categoría |
| Producto concreto | Producto |
| Problema específico | Guía/solución |
| Herramienta/calculadora | Herramienta |

El sistema puede crear tipos adicionales cuando el proyecto lo requiera.

---

# 11. GENERACIÓN DE URL

La URL debe representar claramente la intención y el contenido de la página.

Debe ser:

- comprensible;
- estable;
- corta cuando sea posible;
- coherente con la arquitectura;
- consistente con el resto del proyecto;
- fácil de mantener;
- compatible con el tipo de página.

No debe contener automáticamente todas las keywords detectadas.

---

# 12. ESTRUCTURA DE URL

La estructura debe derivarse de la arquitectura.

Ejemplo:

`/guias/huerto-balcon/`

`/guias/que-necesito-para-pescar-en-rio/`

`/comparativas/mejores-tiendas-de-campana/`

`/productos/kit-supervivencia/`

`/servicios/fontanero/marbella/`

La estructura exacta debe adaptarse al proyecto.

No existe una única estructura universal.

---

# 13. VARIABLES Y PATRONES

Cuando existan combinaciones masivas, el sistema debe identificar patrones.

Ejemplo:

`SERVICIO + LOCALIDAD`

Puede generar:

`/fontanero/marbella/`

`/fontanero/estepona/`

`/fontanero/casares/`

Pero debe evitar generar combinaciones que:

- no tengan sentido;
- no representen una necesidad real;
- sean localidades irrelevantes para el servicio;
- produzcan páginas vacías;
- sean duplicados;
- no puedan aportar valor.

---

# 14. MATRICES

Cuando exista una estructura combinatoria, debe utilizarse una matriz.

Ejemplo:

| Servicio | Localidad | Intención | URL | Estado |
|---|---|---|---|---|
| Fontanero | Marbella | Servicio local | /fontanero/marbella/ | Crear |
| Fontanero | Estepona | Servicio local | /fontanero/estepona/ | Crear |
| Fontanero | Casares | Servicio local | /fontanero/casares/ | Revisar |

La matriz permite separar:

- combinaciones válidas;
- combinaciones dudosas;
- combinaciones descartadas.

---

# 15. WEB DE AFILIACIÓN

Para afiliación, una intención puede producir diferentes soluciones.

Ejemplo:

`qué necesito para pescar en río`

↓

`guía`

↓

`checklist`

↓

`equipamiento`

↓

`productos afiliados`

Puede existir:

`/que-necesito-para-pescar-en-rio/`

Y además, si existe una intención diferenciada:

`/kit-pesca-rio/`

La primera resuelve la necesidad de preparación.

La segunda resuelve la necesidad de encontrar un conjunto de productos.

No deben fusionarse automáticamente.

---

# 16. WEB DE CONTENIDO

En una web de contenido:

`intención`

↓

`problema/pregunta`

↓

`contenido`

↓

`URL`

Ejemplo:

`cómo cultivar tomates en balcón`

↓

`/como-cultivar-tomates-en-balcon/`

Una consulta relacionada como:

`cuándo plantar tomates en balcón`

debe analizarse antes de crear otra URL.

Puede ser:

- una sección;
- una subsección;
- una URL independiente.

La decisión depende de la diferenciación real de la intención.

---

# 17. WEB DE SERVICIOS

En una web de servicios:

`servicio`

+

`localidad`

puede formar una arquitectura válida cuando exista una necesidad local diferenciada.

Ejemplo:

`/fontanero/marbella/`

`/fontanero/estepona/`

Pero el sistema también puede descubrir otras intenciones:

`/fontanero/urgencias/`

`/fontanero/fugas-de-agua/`

`/fontanero/cambio-de-grifo/`

Estas no deben confundirse con las páginas locales.

---

# 18. E-COMMERCE

El sistema debe diferenciar entre:

- categoría;
- subcategoría;
- producto;
- comparativa;
- guía;
- problema;
- necesidad;
- filtro;
- búsqueda interna.

No toda búsqueda de producto debe convertirse en una página indexable.

---

# 19. DIRECTORIOS

En directorios puede existir una combinación de:

`SERVICIO + LOCALIDAD`

pero también:

- categoría;
- especialidad;
- ubicación;
- necesidad;
- características;
- comparaciones.

El sistema debe evitar crear combinaciones sin valor.

---

# 20. PRIORIDAD

Cada URL debe recibir una prioridad.

### P1 — ALTA

Debe crearse primero.

### P2 — MEDIA

Debe crearse después de validar las P1.

### P3 — BAJA

Puede crearse posteriormente.

### P4 — EXPERIMENTAL

Requiere validación adicional.

### DESCARTADA

No crear.

La prioridad debe considerar:

- demanda;
- relevancia;
- monetización;
- dificultad;
- competencia;
- valor;
- coste;
- capacidad de automatización;
- relación con otras URLs.

---

# 21. SALIDA DEL MÓDULO

El resultado debe producir una arquitectura estructurada.

Como mínimo:

| ID | Intención | Keywords | Cluster | Tipo de página | URL | Prioridad | Acción | Justificación |
|---|---|---|---|---|---|---|---|---|
| 001 | ... | ... | ... | ... | ... | P1 | Crear | ... |
| 002 | ... | ... | ... | ... | ... | P2 | Agrupar | ... |
| 003 | ... | ... | ... | ... | ... | P4 | Validar | ... |
| 004 | ... | ... | ... | ... | ... | — | Descartar | ... |

---

# 22. ÁRBOL DE ARQUITECTURA

Cuando sea necesario, convertir la matriz en un árbol.

Ejemplo:

```text
/
├── guias/
│   ├── huerto-balcon/
│   ├── pescar-en-rio/
│   └── supervivencia/
│
├── comparativas/
│   ├── tiendas-campana/
│   └── kits-supervivencia/
│
├── productos/
│   ├── kits-jardineria/
│   └── kits-pesca/
│
└── servicios/
    └── ...

La estructura debe reflejar las necesidades del proyecto.


---

23. CONTROL DE CALIDAD

Antes de aprobar una URL comprobar:

DEMANDA

¿Existe una necesidad real?

INTENCIÓN

¿Está claramente definida?

DIFERENCIACIÓN

¿Es diferente de las URLs existentes?

VALOR

¿La página aportará una respuesta útil?

TIPO

¿El formato de página es adecuado?

URL

¿La URL representa correctamente la página?

ARQUITECTURA

¿Encaja en la estructura general?

MONETIZACIÓN

¿Existe una vía razonable de monetización cuando corresponda?

AUTOMATIZACIÓN

¿Puede generarse manteniendo calidad?

MANTENIMIENTO

¿Será sostenible mantenerla?


---

24. REGLA DE NO GENERACIÓN MASIVA CIEGA

Nunca generar miles de URLs únicamente porque exista una combinación matemática.

Ejemplo:

10 servicios × 500 localidades = 5.000 combinaciones

Esto no significa automáticamente:

5.000 páginas válidas

Cada combinación debe cumplir las reglas del proyecto.

La generación masiva solamente se aprobará cuando exista:

lógica;

demanda o justificación suficiente;

contenido diferenciable;

utilidad;

capacidad de mantenimiento;

control de calidad.



---

25. APRENDIZAJE

La arquitectura no es necesariamente definitiva.

Después de publicar:

DATOS REALES

↓

CONSULTAS REALES

↓

NUEVAS KEYWORDS

↓

NUEVAS INTENCIONES

↓

NUEVAS OPORTUNIDADES

↓

ACTUALIZACIÓN DE ARQUITECTURA

El sistema debe permitir:

crear nuevas URLs;

consolidar URLs;

eliminar URLs;

modificar URLs;

cambiar prioridades;

descubrir nuevos clusters.



---

26. INTEGRACIÓN CON OTROS MÓDULOS

Este módulo debe trabajar junto con:

02-MODULOS/DESCUBRIMIENTO-DEMANDA-E-INTENCIONES.md

y posteriormente con:

módulos de WordPress;

módulos de automatización;

módulos de datos;

analítica;

SEO;

plantillas;

tipos de proyecto.


No sustituye al descubrimiento de demanda.

Lo convierte en una arquitectura ejecutable.


---

27. INTEGRACIÓN CON EL FLUJO GENERAL

El flujo completo queda:

IDEA

↓

ANÁLISIS

↓

VIABILIDAD

↓

DESCUBRIMIENTO DE DEMANDA

↓

KEYWORDS

↓

INTENCIONES

↓

CLUSTERS

↓

OPORTUNIDADES

↓

GENERACIÓN DE ARQUITECTURA

↓

TIPOS DE PÁGINA

↓

URLS

↓

PLANTILLAS

↓

CONTENIDO / DATOS

↓

CONSTRUCCIÓN

↓

PUBLICACIÓN

↓

DATOS REALES

↓

MEJORA


---

28. REGLA PARA LA IA

Cuando reciba una idea de proyecto, la IA debe determinar primero si:

A. las URLs ya están suficientemente definidas;

o

B. es necesario descubrirlas.

Si es A:

VALIDAR → AMPLIAR SI PROCEDE → ARQUITECTURA

Si es B:

DESCUBRIR → INTERPRETAR → AGRUPAR → PRIORIZAR → ARQUITECTURA

La IA no debe inventar volumen de búsqueda ni otras métricas.

Cuando necesite datos externos debe:

obtenerlos mediante una fuente disponible;

o solicitar al usuario los datos necesarios.



---

29. RESULTADO FINAL

El módulo debe ser capaz de recibir:

> una idea de negocio o proyecto



y producir:

> una estructura razonada de páginas y URLs basada en las necesidades e intenciones detectadas.



El resultado no debe ser simplemente una lista de keywords.

Debe explicar:

qué busca el usuario;

qué intención representa;

qué problema existe;

qué solución se propone;

qué página debe responder;

qué URL tendrá;

por qué merece existir;

qué prioridad tiene;

cómo encaja en la arquitectura.



---

30. REGLA FINAL

El objetivo no es crear muchas URLs.

El objetivo es crear:

las URLs correctas para las necesidades correctas.

Por tanto:

DEMANDA → INTENCIÓN → OPORTUNIDAD → PÁGINA → URL → ARQUITECTURA

La cantidad de URLs será una consecuencia del mercado y del proyecto, nunca el objetivo principal.


