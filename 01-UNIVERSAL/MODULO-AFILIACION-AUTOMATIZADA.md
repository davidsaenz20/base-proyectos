
MÓDULO DE AFILIACIÓN AUTOMATIZADA

PROPÓSITO

Definir el comportamiento reutilizable para proyectos basados en marketing de afiliación, tanto de productos como de servicios, incluyendo proyectos automatizados o semiautomatizados y modelos de flotilla de múltiples webs.

Este módulo debe utilizarse cuando un proyecto pretenda monetizar mediante comisiones generadas por ventas, leads, reservas, contrataciones, registros u otras acciones atribuidas a enlaces o sistemas de afiliación.

No está limitado a Amazon ni a ninguna red concreta.

---

1. PRINCIPIO GENERAL

La afiliación debe tratarse como un modelo de negocio, no como una tecnología concreta.

La IA debe investigar primero qué redes, anunciantes, programas, APIs y feeds existen y posteriormente decidir qué combinación resulta más adecuada.

Nunca debe asumirse que Amazon es la única fuente posible.

Las fuentes pueden incluir, cuando sean legal y técnicamente utilizables:

- programas directos de marcas;
- redes de afiliación;
- marketplaces de afiliación;
- plataformas de viajes;
- vuelos;
- hoteles;
- alquiler de vehículos;
- seguros;
- software;
- servicios profesionales;
- generación de leads;
- productos físicos;
- productos digitales;
- suscripciones;
- otros servicios comercializables mediante afiliación.

---

2. REQUISITO DE COSTE DE AFILIACIÓN

Por defecto, el sistema debe priorizar programas que permitan registrarse como publisher/affiliate sin pagar una cuota de afiliación.

El requisito operativo es:

«NO pagar por afiliarse.»

Debe distinguirse entre:

- cuota de alta o afiliación;
- depósito de verificación;
- herramientas opcionales de pago;
- costes de dominio/hosting;
- costes de IA;
- costes de automatización;
- otros costes operativos.

Una plataforma que sea gratuita pero exija un depósito temporal debe clasificarse como:

🟡 CASI GRATUITA / REQUIERE VERIFICACIÓN

No debe presentarse como coste cero absoluto.

Una plataforma que cobre una cuota obligatoria de acceso debe quedar descartada salvo autorización expresa del usuario.

---

3. INVESTIGACIÓN OBLIGATORIA ANTES DE CONSTRUIR

Cuando se proponga una web de afiliación, antes de construir debe investigarse:

Plataforma / red

- nombre;
- países disponibles;
- mercados disponibles;
- requisitos para publishers;
- dificultad de aprobación;
- tiempo aproximado de aprobación;
- existencia de aprobación de la red y aprobación independiente del anunciante;
- costes de afiliación;
- métodos de pago;
- umbral de pago.

Programa / anunciante

- anunciante;
- país objetivo;
- categorías;
- catálogo;
- número aproximado de productos o servicios;
- comisión;
- comisión fija o porcentual;
- cookie/duración de atribución cuando sea relevante;
- condiciones;
- restricciones;
- fuentes de tráfico permitidas;
- restricciones SEO/PPC cuando existan;
- posibilidad de comparadores;
- posibilidad de páginas de contenido;
- posibilidad de utilizar feeds;
- disponibilidad de API;
- frecuencia de actualización;
- calidad de imágenes y datos;
- disponibilidad de enlaces profundos.

---

4. PRODUCT FEEDS Y SERVICE FEEDS

Cuando exista catálogo estructurado, la IA debe priorizar fuentes que permitan obtener datos automáticamente.

Los datos pueden incluir, según disponibilidad:

- identificador del producto/servicio;
- SKU/ASIN u otro identificador;
- nombre;
- descripción;
- precio;
- precio anterior;
- moneda;
- descuento;
- imagen;
- imágenes adicionales;
- disponibilidad;
- stock;
- marca;
- categoría;
- atributos;
- URL de destino;
- enlace profundo de afiliado;
- país;
- fecha de actualización.

La IA debe comprobar qué campos proporciona realmente cada fuente.

Nunca debe inventar campos que el feed no proporcione.

---

5. API Y AUTOMATIZACIÓN

Cuando exista API oficial debe estudiarse antes de desarrollar scraping.

Prioridad:

1. API oficial;
2. feed oficial;
3. exportación oficial programable;
4. integración oficial mediante FTP u otro mecanismo documentado;
5. automatización autorizada de plataforma;
6. scraping únicamente si es legal, permitido por las condiciones aplicables y técnicamente necesario.

No se debe construir una dependencia de scraping si existe una API/feed oficial adecuado.

---

6. MODELO DE DATOS UNIVERSAL

El sistema debe normalizar los datos de diferentes redes en un modelo interno común.

Ejemplo conceptual:

affiliate_item_id
source
merchant
country
category
name
description
image_url
price
old_price
currency
availability
brand
product_url
affiliate_url
commission_type
commission_value
last_updated
status

Para servicios pueden utilizarse campos equivalentes:

service_id
provider
service_type
country
city
name
description
image_url
landing_url
affiliate_url
commission_type
commission_value
lead_value
last_updated
status

La arquitectura debe permitir incorporar nuevas redes sin rediseñar el sistema completo.

---

7. MODELO MULTIPROVEEDOR

No debe diseñarse el sistema alrededor de una sola red.

Arquitectura recomendada:

RED A ─┐
RED B ─┤
RED C ─┤
RED D ─┤→ NORMALIZACIÓN → MOTOR DE AFILIACIÓN → WEB
RED E ─┘

El sistema debe permitir:

- añadir fuentes;
- eliminar fuentes;
- sustituir fuentes;
- priorizar fuentes;
- detectar productos duplicados;
- seleccionar la mejor oferta disponible;
- mantener histórico de fuente y actualización.

---

8. PRODUCTOS Y SERVICIOS

El módulo no se limita a tiendas de productos.

Debe poder utilizarse para:

- comercio electrónico;
- comparadores;
- vuelos;
- hoteles;
- viajes;
- alquiler de coches;
- seguros;
- software;
- SaaS;
- cursos;
- servicios profesionales;
- telecomunicaciones;
- energía;
- finanzas cuando sea legal y apropiado;
- generación de leads;
- reservas;
- suscripciones.

La estructura debe adaptarse al modelo de comisión de cada sector.

---

9. COMISIONES

Una comisión baja no implica automáticamente que el proyecto sea inviable.

La rentabilidad debe analizarse mediante:

INGRESO ESPERADO
=
TRÁFICO
× CTR AFILIADO
× CONVERSIÓN
× VALOR MEDIO DE COMISIÓN

También deben considerarse:

- recurrencia;
- duración de cookie/atribución;
- cancelaciones;
- devoluciones;
- porcentaje de aprobación de transacciones;
- valor medio del pedido;
- comisión fija;
- comisión porcentual;
- recurrencia de la comisión;
- vida útil del cliente cuando corresponda.

Una comisión porcentualmente pequeña puede ser interesante si el ticket, volumen o conversión son elevados.

Una comisión alta puede ser poco interesante si existe poca demanda o una conversión muy baja.

---

10. MODELO FLOTILLA

El sistema debe contemplar expresamente un segundo modelo de negocio:

«FLOTA DE WEBS AFILIADAS.»

En este modelo no es obligatorio que cada web produzca grandes beneficios individualmente.

La unidad económica mínima es:

INGRESOS DE LA WEB
>
COSTE ANUAL REAL DE MANTENERLA

Una web puede mantenerse si cubre razonablemente:

- dominio;
- hosting atribuible;
- automatización atribuible;
- IA atribuible;
- otros costes directos.

Las webs que no cubran sus costes después del periodo de validación deben poder marcarse para:

- optimización;
- cambio de estrategia;
- cambio de monetización;
- cambio de nicho;
- venta;
- cierre;
- no renovación del dominio.

No se debe renovar automáticamente una web únicamente porque exista.

---

11. ESCALABILIDAD

Antes de recomendar una flotilla, calcular:

- tiempo humano por web;
- coste de creación por web;
- coste mensual por web;
- coste anual por web;
- coste de mantenimiento;
- coste de actualización de contenidos;
- coste de IA;
- coste de productos/feeds;
- coste de hosting;
- coste de dominios;
- dependencia de APIs externas.

El objetivo es reducir el coste marginal de cada nueva web.

La IA debe buscar reutilización de:

- plantillas;
- componentes;
- workflows n8n;
- conectores;
- modelos de datos;
- prompts;
- bloques WordPress;
- estructuras SEO;
- procesos de actualización;
- validaciones.

---

12. CRITERIO DE SELECCIÓN DE OPORTUNIDADES

Una oportunidad de afiliación debe evaluarse como mínimo mediante:

OPORTUNIDAD
↓
DEMANDA
↓
COMPETENCIA
↓
PROGRAMAS
↓
APROBACIÓN
↓
CATÁLOGO
↓
FEED/API
↓
ACTUALIZACIÓN
↓
COMISIÓN
↓
COSTE
↓
AUTOMATIZACIÓN
↓
ESCALABILIDAD
↓
RIESGO
↓
VIABILIDAD

La IA debe buscar alternativas si el primer programa o nicho no es suficientemente atractivo.

---

13. NO CONSTRUIR ANTES DE VALIDAR

No debe iniciarse la construcción completa de una web afiliada únicamente porque exista un catálogo.

Debe comprobarse previamente que:

- existe programa afiliado válido;
- el publisher puede registrarse sin coste obligatorio;
- el mercado objetivo está cubierto;
- el catálogo es suficiente;
- los datos son utilizables;
- la actualización es viable;
- las condiciones permiten el modelo previsto;
- existe una hipótesis razonable de rentabilidad;
- la automatización puede reducir suficientemente el coste.

Cuando estos puntos no estén claros, el trabajo debe permanecer en estudio previo.

---

14. APROBACIÓN Y ACCESO

La IA debe distinguir siempre:

A. aprobación de la red;

B. aprobación del publisher/canal;

C. aprobación de cada anunciante/programa.

No debe asumir que entrar en una red significa tener acceso a todos sus anunciantes.

Cuando una oportunidad dependa de la aprobación de un anunciante, debe registrarse como riesgo o dependencia.

---

15. CUMPLIMIENTO Y DATOS

Solo deben utilizarse datos de productos y servicios mediante mecanismos permitidos por la plataforma, anunciante y normativa aplicable.

La IA debe comprobar las condiciones de uso del feed/API y las restricciones sobre:

- almacenamiento;
- caché;
- imágenes;
- precios;
- marcas;
- textos;
- enlaces;
- SEO;
- PPC;
- redirecciones;
- comparadores;
- uso automatizado.

Los precios, disponibilidad y demás datos sensibles deben tratarse como datos potencialmente caducos.

Cuando el proveedor permita actualización automática, el sistema debe registrar "last_updated" y disponer de un proceso de sincronización.

---

16. WORDPRESS + N8N

Arquitectura recomendada:

FUENTES DE AFILIACIÓN
        ↓
       N8N
        ↓
NORMALIZACIÓN / FILTRADO
        ↓
BASE DE DATOS / DATASET
        ↓
IA + REGLAS
        ↓
CONTENIDO / PRODUCTOS / SERVICIOS
        ↓
WORDPRESS
        ↓
KADENCE / BLOQUES
        ↓
PUBLICACIÓN
        ↓
SINCRONIZACIÓN

n8n debe utilizarse para orquestación y sincronización.

WordPress debe utilizarse para publicación y presentación.

La lógica de negocio crítica no debe quedar dispersa entre cientos de páginas manuales.

---

17. ACTUALIZACIÓN AUTOMÁTICA

El sistema debe separar:

Datos dinámicos

- precio;
- stock;
- disponibilidad;
- descuento;
- enlace;
- fecha de actualización.

Contenido editorial

- textos;
- comparativas;
- guías;
- explicaciones;
- estructura SEO.

Los datos dinámicos deben poder actualizarse sin regenerar necesariamente todo el contenido editorial.

---

18. DECISIÓN DEL SISTEMA

La IA debe terminar el análisis con una recomendación de:

🟢 VIABLE

🟡 VIABLE CONDICIONALMENTE

🟠 REQUIERE VALIDACIÓN

🔴 NO VIABLE

Pero esta recomendación no sustituye la decisión del usuario.

El usuario decide si:

- construir;
- construir un MVP;
- construir una flotilla piloto;
- modificar el modelo;
- investigar más;
- abandonar.

---

19. MÉTRICAS DE VALIDACIÓN

Una web afiliada piloto debe poder medirse mediante:

- visitas;
- páginas indexadas;
- impresiones;
- clics afiliados;
- CTR afiliado;
- conversiones;
- comisión generada;
- EPC cuando esté disponible;
- coste mensual;
- coste anual;
- beneficio neto estimado;
- tiempo humano invertido;
- coste de IA;
- coste de infraestructura.

La decisión de renovar o cerrar debe basarse en datos.

---

20. PRINCIPIO FINAL

El objetivo no es crear miles de webs porque técnicamente sea posible.

El objetivo es construir un sistema capaz de:

1. descubrir oportunidades de afiliación;
2. investigar su viabilidad;
3. encontrar programas y fuentes sin coste obligatorio de afiliación;
4. obtener productos o servicios mediante feeds/APIs cuando sea posible;
5. automatizar la creación y actualización;
6. reducir el coste marginal de cada web;
7. medir resultados;
8. conservar las webs que funcionan;
9. mejorar las webs con potencial;
10. cerrar las que no justifican su coste;
11. repetir el proceso con nuevas oportunidades.

La ventaja competitiva buscada es el sistema de descubrimiento, validación, construcción, automatización y gestión de una cartera de webs, no la dependencia de una red concreta.


