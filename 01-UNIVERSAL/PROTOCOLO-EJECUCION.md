# PROTOCOLO DE EJECUCIÓN

## Objetivo

Definir el proceso para ejecutar un proyecto desde la idea inicial hasta su validación y puesta en funcionamiento.

El protocolo debe permitir adaptar el proceso al tipo de proyecto sin perder control, trazabilidad, validación ni capacidad de reutilización.

---

# FASES

1. Analizar la idea.
2. Evaluar viabilidad.
3. Definir requisitos.
4. Determinar necesidades de investigación.
5. Descubrir y validar demanda cuando corresponda.
6. Definir las intenciones y oportunidades cuando corresponda.
7. Tomar decisiones.
8. Diseñar la arquitectura.
9. Seleccionar módulos y plantillas.
10. Planificar la implementación.
11. Construir.
12. Probar.
13. Corregir.
14. Validar.
15. Desplegar.
16. Monitorizar.
17. Mejorar.

Cada fase debe producir un resultado verificable antes de considerar que la fase está completada.

El proceso debe avanzar de forma iterativa cuando una prueba detecte errores, nueva información o nuevas necesidades.

---

# 1. ANALIZAR LA IDEA

Determinar:

- qué se quiere construir;
- qué problema se pretende resolver;
- quién es el usuario;
- cuál es el resultado esperado;
- cuál es el modelo de negocio cuando corresponda;
- qué hipótesis existen;
- qué información falta;
- qué decisiones deberán tomarse.

No comenzar la construcción mientras existan incertidumbres fundamentales que puedan cambiar la solución.

---

# 2. EVALUAR VIABILIDAD

Realizar el estudio previo correspondiente.

Evaluar, cuando sea aplicable:

- demanda;
- competencia;
- oportunidad;
- modelo de negocio;
- monetización;
- costes;
- recursos;
- tecnología;
- riesgos;
- capacidad de ejecución;
- escalabilidad;
- requisitos legales;
- dependencias.

Cuando el proyecto dependa de tráfico procedente de búsquedas, la existencia de demanda debe investigarse de acuerdo con las reglas de descubrimiento de demanda.

---

# 3. DEFINIR REQUISITOS

Definir los requisitos funcionales y no funcionales.

Los requisitos deben indicar, cuando corresponda:

- usuarios;
- funcionalidades;
- contenido;
- datos;
- integraciones;
- monetización;
- SEO;
- páginas;
- arquitectura;
- automatizaciones;
- seguridad;
- analítica;
- criterios de éxito.

Los requisitos pueden modificarse si una investigación posterior demuestra que la hipótesis inicial era incorrecta.

---

# 4. DETERMINAR LAS NECESIDADES DE INVESTIGACIÓN

Antes de diseñar la arquitectura debe determinarse qué información necesita el proyecto para tomar decisiones correctamente.

Preguntas mínimas:

- ¿La demanda ya está definida?
- ¿Las necesidades de los usuarios son conocidas?
- ¿Las URLs ya están justificadas?
- ¿Existe una matriz predeterminada?
- ¿El proyecto depende de SEO?
- ¿Depende de búsquedas de usuarios?
- ¿Necesitamos descubrir problemas o necesidades?
- ¿Necesitamos descubrir keywords?
- ¿Necesitamos analizar intenciones?
- ¿Necesitamos descubrir nuevas oportunidades?

El objetivo es evitar tanto la investigación insuficiente como la investigación innecesaria.

---

# 5. DESCUBRIMIENTO Y VALIDACIÓN DE DEMANDA

## 5.1 CUÁNDO ACTIVAR EL MÓDULO

Cuando el proyecto dependa de conocer qué buscan o necesitan los usuarios, debe utilizarse:

`02-MODULOS/DESCUBRIMIENTO-DEMANDA-E-INTENCIONES.md`

Esto incluye, entre otros:

- webs de afiliación;
- webs de contenido;
- generación de leads;
- servicios;
- e-commerce;
- directorios;
- comparadores;
- marketplaces;
- proyectos locales;
- SaaS dependientes de adquisición orgánica;
- herramientas o recursos basados en búsquedas;
- otros proyectos donde las búsquedas determinen la arquitectura o adquisición.

---

## 5.2 DETERMINAR SI LA DEMANDA YA ESTÁ ESTRUCTURADA

Debe distinguirse entre dos situaciones.

### CASO A — DEMANDA O ESTRUCTURA PREDEFINIDA

Si el proyecto dispone de una estructura previamente justificada, puede utilizarse como punto de partida.

Ejemplo:

`servicio + localidad`

En este caso no es obligatorio descubrir desde cero todas las URLs mediante keyword research.

Sin embargo, puede realizarse investigación para:

- validar la estructura;
- detectar variantes;
- detectar nuevas intenciones;
- descubrir oportunidades;
- priorizar;
- evitar páginas innecesarias;
- mejorar la arquitectura.

### CASO B — DEMANDA NO DEFINIDA

Si todavía no se conoce:

- qué busca el usuario;
- qué problemas tiene;
- qué necesidades existen;
- qué soluciones espera;
- qué páginas deberían existir;

debe ejecutarse el módulo de descubrimiento de demanda antes de fijar definitivamente la arquitectura.

---

# 6. PROCESO DE DESCUBRIMIENTO DE DEMANDA

Cuando corresponda:

IDEA

↓

PROBLEMA / MERCADO

↓

INVESTIGACIÓN DE DEMANDA

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

---

# 7. REGLA KEYWORD → INTENCIÓN → URL

Nunca debe aplicarse:

`1 keyword = 1 URL`

Una keyword es una señal.

Una intención representa una necesidad o resultado que busca el usuario.

Una URL debe existir cuando exista una razón real para que esa página satisfaga una intención diferenciada.

Por tanto:

`KEYWORD ≠ INTENCIÓN ≠ URL`

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

# 9. DECIDIR LAS URLS

A partir de las intenciones y oportunidades debe determinarse:

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

Cuando el proyecto dependa de la generación o reorganización de URLs a partir de intenciones de búsqueda, debe utilizarse:

`02-MODULOS/GENERACION-ARQUITECTURA-URLS-POR-INTENCION.md`

Este módulo convierte las intenciones y oportunidades detectadas en:

- decisiones de páginas;
- agrupaciones;
- URLs;
- tipos de página;
- prioridades;
- arquitectura.

La decisión debe realizarse antes de pasar a la selección definitiva de plantillas y construcción.

---

# 10. DECISIONES

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

# 11. DISEÑAR LA ARQUITECTURA

La arquitectura debe diseñarse después de disponer de la información necesaria para determinar qué debe existir.

Cuando el proyecto dependa de demanda:

DEMANDA

↓

INTENCIONES

↓

CLUSTERS

↓

OPORTUNIDADES

↓

TIPOS DE PÁGINA

↓

ARQUITECTURA

Cuando exista una estructura predeterminada y justificada:

ESTRUCTURA

↓

VALIDACIÓN

↓

ARQUITECTURA

---

# 12. SELECCIONAR MÓDULOS Y PLANTILLAS

Antes de construir:

1. identificar el tipo de proyecto;
2. consultar `04-TIPOS-PROYECTO/`;
3. identificar módulos necesarios en `02-MODULOS/`;
4. identificar plantillas aplicables en `03-PLANTILLAS/`;
5. comprobar que no exista documentación equivalente;
6. definir las dependencias.

El módulo de descubrimiento de demanda debe activarse cuando las condiciones descritas anteriormente lo requieran.

---

# 13. DISEÑO DE PÁGINAS Y PLANTILLAS

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

`INTENCIÓN TRANSACCIONAL → PLANTILLA COMERCIAL`

`INTENCIÓN LOCAL → PLANTILLA LOCAL`

Una misma plantilla puede reutilizarse cuando realmente sea adecuada.

---

# 14. PLANIFICAR LA IMPLEMENTACIÓN

Definir:

- orden de construcción;
- dependencias;
- automatizaciones;
- fuentes de datos;
- herramientas;
- APIs;
- WordPress u otra tecnología;
- generación de contenido;
- generación de páginas;
- analítica;
- validaciones.

Cuando existan muchas URLs, priorizar por:

- oportunidad;
- demanda;
- dificultad;
- valor comercial;
- capacidad de conversión;
- recursos necesarios.

No es obligatorio construir todas las URLs de una vez.

---

# 15. CONSTRUIR

Construir siguiendo:

- requisitos;
- decisiones;
- arquitectura;
- tipo de proyecto;
- módulos;
- plantillas;
- reglas de calidad.

Cuando el proyecto sea escalable, reutilizar componentes y automatizaciones.

La automatización no debe generar páginas únicamente por volumen.

Cada página debe tener una función definida.

---

# 16. PROBAR

Ejecutar las pruebas correspondientes.

Comprobar, cuando aplique:

- funcionalidad;
- arquitectura;
- navegación;
- contenido;
- SEO;
- datos;
- automatizaciones;
- integraciones;
- rendimiento;
- seguridad;
- conversión.

---

# 17. CORREGIR

Cuando una prueba detecte un problema:

1. registrar el problema;
2. identificar la causa;
3. determinar la corrección;
4. aplicar la corrección;
5. repetir la prueba.

Si el problema procede de una hipótesis de demanda incorrecta:

DATOS

↓

NUEVA INVESTIGACIÓN

↓

NUEVA INTENCIÓN

↓

NUEVA DECISIÓN

↓

CORRECCIÓN

↓

VALIDACIÓN

---

# 18. VALIDAR

La fase se considera completada cuando existe evidencia suficiente de que el resultado cumple los criterios definidos.

No basta con que el sistema funcione técnicamente.

Debe comprobarse también que resuelve el problema previsto.

---

# 19. VALIDACIÓN DE PROYECTOS BASADOS EN SEO

Cuando el proyecto dependa de búsquedas, después de publicar deben analizarse:

- impresiones;
- clics;
- posiciones;
- consultas reales;
- nuevas keywords;
- nuevas intenciones;
- páginas con tráfico;
- páginas sin tráfico;
- conversiones;
- comportamiento del usuario.

Los datos reales pueden modificar la arquitectura futura.

---

# 20. DESPLEGAR

Realizar el despliegue previsto cuando:

- las pruebas necesarias hayan sido superadas;
- los errores críticos estén resueltos;
- la configuración esté comprobada;
- la medición esté preparada.

---

# 21. MONITORIZAR

Monitorizar:

- errores;
- rendimiento;
- tráfico;
- conversiones;
- costes;
- disponibilidad;
- seguridad;
- comportamiento;
- resultados SEO;
- nuevas oportunidades.

---

# 22. MEJORAR

Los datos obtenidos deben alimentar nuevamente el sistema.

Ejemplo:

PUBLICACIÓN

↓

DATOS REALES

↓

NUEVAS CONSULTAS

↓

NUEVAS INTENCIONES

↓

NUEVAS OPORTUNIDADES

↓

MEJORA

↓

NUEVAS PÁGINAS / CAMBIOS

---

# CONTROL DEL PROYECTO

El estado del proyecto debe mantenerse sincronizado con:

- `00-CONTROL/ESTADO.md`
- `00-CONTROL/ROADMAP.md`
- `00-CONTROL/DECISIONES.md`
- `00-CONTROL/INVENTARIO-DOCUMENTOS.md`

---

# USO DE PLANTILLAS

Las plantillas de `03-PLANTILLAS/` deben reutilizarse cuando sean aplicables.

No se debe crear una estructura nueva si una plantilla existente puede resolver la necesidad sin introducir complejidad innecesaria.

---

# USO DE MÓDULOS

Los módulos de `02-MODULOS/` deben utilizarse cuando aporten una capacidad necesaria para el proyecto.

Los módulos deben mantenerse independientes y reutilizables siempre que sea posible.

No se deben duplicar módulos para resolver una misma función.

---

# TIPO DE PROYECTO

Antes de iniciar la construcción debe identificarse el tipo de proyecto y consultar el documento correspondiente dentro de:

`04-TIPOS-PROYECTO/`

---

# FIXTURES

Cuando exista un fixture aplicable en:

`05-FIXTURES/`

debe utilizarse para validar que la metodología puede ejecutarse correctamente.

---

# VALIDACIÓN DEL PROCESO

La finalización de una fase no debe basarse únicamente en que exista documentación.

Debe existir evidencia suficiente de que el resultado funciona según los requisitos definidos.

---

# CRITERIO DE FINALIZACIÓN

Un proyecto solo puede considerarse finalizado cuando:

- los requisitos principales están cubiertos;
- las decisiones importantes están registradas;
- las investigaciones necesarias se han realizado;
- las hipótesis críticas han sido validadas cuando corresponda;
- las pruebas necesarias se han ejecutado;
- los errores críticos están resueltos;
- el despliegue previsto se ha realizado cuando corresponda;
- el resultado ha sido validado;
- la documentación necesaria está actualizada.

---

# REGLA FINAL

El protocolo debe responder siempre a cuatro preguntas:

1. ¿Qué problema estamos resolviendo?
2. ¿Qué evidencia tenemos?
3. ¿Qué debemos construir?
4. ¿Cómo sabremos que funciona?

Cuando las respuestas dependan de conocer qué buscan o necesitan los usuarios, debe utilizarse:

`02-MODULOS/DESCUBRIMIENTO-DEMANDA-E-INTENCIONES.md`

Cuando la demanda o estructura ya esté suficientemente definida, no debe realizarse investigación redundante.

La investigación debe ser proporcional a la incertidumbre.

La arquitectura debe derivarse de las necesidades reales del proyecto.

La automatización debe escalar valor, no únicamente volumen.


