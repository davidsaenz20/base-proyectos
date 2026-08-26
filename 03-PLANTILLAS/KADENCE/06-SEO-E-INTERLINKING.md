06-SEO-E-INTERLINKING.md

# KADENCE — SEO E INTERLINKING

## Propósito

Documentar cómo construir la estructura SEO e interlinking de las webs utilizando WordPress + Kadence, diferenciando claramente las funciones del tema de las funciones de WordPress y de los plugins SEO.

---

# 1. PRINCIPIO GENERAL

Kadence se utiliza principalmente para:

- estructura visual;
- layouts;
- navegación;
- menús;
- bloques;
- enlaces;
- responsive;
- presentación del contenido.

El SEO específico puede depender de WordPress y de un plugin SEO.

No atribuir a Kadence funcionalidades que pertenezcan realmente a otro componente del stack.

---

# 2. ARQUITECTURA ANTES DE CONSTRUIR

Antes de crear páginas definir:

- página principal;
- páginas de servicios;
- páginas de localidades;
- páginas informativas;
- categorías;
- páginas legales;
- estructura de navegación;
- jerarquía;
- enlaces internos.

La arquitectura debe definirse antes de crear cientos de páginas.

---

# 3. ESTRUCTURA DE URL

Las URLs deben ser:

- cortas;
- descriptivas;
- estables;
- legibles;
- coherentes;
- orientadas al contenido.

Evitar cambiar URLs después de que una página haya sido publicada e indexada salvo que exista una razón justificada.

---

# 4. MENÚ PRINCIPAL

El menú principal debe contener únicamente las páginas más importantes.

No utilizar el menú como sistema para enlazar todas las páginas existentes.

Debe priorizar:

- páginas principales;
- servicios principales;
- información esencial;
- contacto;
- categorías estratégicas.

---

# 5. INTERLINKING CONTEXTUAL

Los enlaces internos deben aparecer también dentro del contenido.

Ejemplos:

- una página de servicio enlaza a servicios relacionados;
- una página local enlaza a localidades cercanas;
- una página informativa enlaza a servicios relevantes;
- una página secundaria enlaza hacia su página principal.

El anchor text debe describir razonablemente el destino.

---

# 6. BLOQUES PARA INTERLINKING

Se pueden utilizar:

- botones;
- listas;
- tarjetas;
- enlaces de texto;
- bloques de servicios;
- bloques relacionados;
- navegación contextual.

No crear enlaces únicamente para aumentar artificialmente el número de enlaces internos.

---

# 7. BREADCRUMBS

Cuando la arquitectura del proyecto lo requiera, utilizar breadcrumbs.

Deben reflejar la jerarquía real.

Ejemplo:

```text
Inicio
→ Servicios
→ Fontanería
→ Fontanero Marbella

La implementación concreta dependerá del stack SEO utilizado.


---

8. ENLACES ENTRE LOCALIDADES

En proyectos de SEO local:

evitar enlazar indiscriminadamente todas las localidades entre sí;

priorizar relaciones geográficas y temáticas reales;

evitar crear redes artificiales de enlaces;

mantener una estructura lógica.



---

9. ENLACES ENTRE SERVICIOS

Cuando varios servicios estén relacionados:

Servicio principal
↓
Servicios relacionados
↓
Contenido informativo
↓
Contacto / conversión

La relación debe aportar utilidad al usuario.


---

10. H1

Cada página debe tener una jerarquía clara.

Como regla general:

un H1 principal;

H2 para secciones;

H3 para subsecciones;

no utilizar headings únicamente por estética.


El diseño visual y la jerarquía semántica son conceptos diferentes.


---

11. IMÁGENES

Las imágenes deben disponer de:

nombre de archivo descriptivo cuando corresponda;

texto alternativo adecuado;

tamaño optimizado;

formato apropiado.


No utilizar texto alternativo para introducir palabras clave artificialmente.


---

12. META TITLE Y META DESCRIPTION

La gestión concreta depende del plugin SEO utilizado.

Para cada página definir:

keyword/intención principal;

title;

meta description;

URL;

H1;

estructura de headings.


Evitar duplicaciones innecesarias.


---

13. CANONICAL

Cuando existan páginas similares, comprobar la canonical correspondiente.

Especialmente importante en proyectos con generación automática de páginas.

No crear miles de URLs casi idénticas sin justificar su existencia.


---

14. PÁGINAS GENERADAS AUTOMÁTICAMENTE

Si n8n genera páginas:

Antes de publicar cada página comprobar:

contenido único;

intención de búsqueda;

utilidad real;

URL correcta;

title;

H1;

enlaces internos;

imágenes;

datos del negocio;

localidad;

ausencia de contenido duplicado.


No publicar automáticamente una página únicamente porque sea posible generarla.


---

15. INTERLINKING AUTOMÁTICO

Cuando exista generación automática de enlaces:

Definir reglas claras.

Ejemplo:

Página de servicio
→ página principal del servicio

Página local
→ servicio de la localidad

Página de localidad
→ localidades relacionadas

Contenido informativo
→ servicio relacionado

Las reglas deben evitar enlaces excesivos o irrelevantes.


---

16. MAPA DE ENLACES

Para proyectos grandes crear una matriz lógica:

PÁGINA
↓
ENLAZA A
↓
MOTIVO
↓
ANCHOR

Ejemplo:

Fontanero Marbella
→ Reparación de fugas
→ Servicio relacionado
→ "reparación de fugas de agua"


---

17. ENLACES ROTOS

Antes de publicar:

comprobar enlaces internos;

comprobar enlaces externos;

comprobar páginas eliminadas;

comprobar redirecciones;

comprobar anchors.


Después de publicar, realizar comprobaciones periódicas cuando el proyecto lo requiera.


---

18. CAMBIOS DE URL

Si una URL publicada cambia:

1. registrar la URL antigua;


2. definir la nueva;


3. crear redirección si corresponde;


4. actualizar enlaces internos;


5. comprobar indexación posteriormente.



No modificar URLs sin motivo.


---

19. SEO LOCAL

Cuando el proyecto tenga orientación local, documentar:

servicio;

localidad;

áreas atendidas;

información de contacto;

datos coherentes;

páginas locales;

interlinking geográfico;

contenido específico.


No crear páginas locales prácticamente idénticas cambiando únicamente el nombre de la localidad.


---

20. REGLA CONTRA PÁGINAS VACÍAS

Una página debe existir porque satisface una necesidad real del usuario.

Antes de generar páginas masivamente preguntar:

> ¿Esta página tiene una intención de búsqueda y una utilidad diferenciada?



Si la respuesta es no:

no generar automáticamente.


---

21. VALIDACIÓN SEO BÁSICA

Antes de considerar terminada una página:

[ ] URL correcta

[ ] H1 correcto

[ ] H2/H3 coherentes

[ ] title definido

[ ] meta description definida cuando corresponda

[ ] contenido útil

[ ] enlaces internos relevantes

[ ] enlaces funcionando

[ ] imágenes optimizadas

[ ] alt text adecuado

[ ] canonical comprobada cuando corresponda

[ ] responsive correcto



---

22. REGLA OPERATIVA

Cuando el usuario tenga que configurar algo relacionado con SEO o interlinking, indicar:

OBJETIVO

Qué queremos conseguir.

COMPONENTE

WordPress / Kadence / plugin SEO / n8n.

RUTA

Dónde entrar.

CAMBIO

Qué modificar.

VALOR

Qué introducir.

VERIFICACIÓN

Qué comprobar.


---

23. AUTOMATIZACIÓN CON N8N

Cuando n8n participe en la creación o actualización de páginas, separar:

DATOS
↓
GENERACIÓN
↓
VALIDACIÓN
↓
PUBLICACIÓN
↓
INDEXACIÓN
↓
MONITORIZACIÓN

No permitir que la automatización publique contenido sin controles de calidad definidos.


---

24. PRINCIPIO FINAL

El SEO no consiste en crear el mayor número posible de páginas.

El objetivo es crear:

la página correcta + para la intención correcta + con contenido útil + dentro de una arquitectura lógica.

El interlinking debe ayudar al usuario y a los buscadores a comprender esa arquitectura.



