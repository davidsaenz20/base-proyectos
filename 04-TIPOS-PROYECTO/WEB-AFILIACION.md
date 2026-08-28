# WEB DE AFILIACIÓN

## 1. PROPÓSITO

Definir la metodología específica para crear, validar, automatizar, lanzar, medir y escalar una web de afiliación.

Este documento adapta el sistema general de trabajo a proyectos cuyo modelo de monetización principal o complementario sea la afiliación.

La web debe construirse para resolver necesidades reales de los usuarios y convertir esas soluciones en oportunidades de monetización.

El objetivo no es crear muchas páginas.

El objetivo es crear un activo digital útil que pueda adquirir tráfico cualificado, generar clics, conversiones e ingresos.

---

# 2. PRINCIPIO FUNDAMENTAL

Una web de afiliación no debe comenzar necesariamente por los productos.

Debe comenzar por:

PROBLEMA / NECESIDAD
↓
INTENCIÓN
↓
SOLUCIÓN
↓
PRODUCTOS / SERVICIOS
↓
AFILIACIÓN
↓
CONVERSIÓN
↓
INGRESOS

Los productos son una posible solución a una necesidad.

Por tanto, la arquitectura de la web debe organizarse alrededor de las necesidades del usuario siempre que tenga sentido.

---

# 3. RELACIÓN CON EL SISTEMA GENERAL

Este documento no funciona de forma aislada.

Debe utilizar los módulos generales del repositorio.

Especialmente:

- módulo de descubrimiento de demanda e intenciones;
- módulo de afiliación;
- módulo de automatización;
- módulo de contenidos;
- módulo de SEO;
- módulo de validación;
- módulo de analítica;
- módulos técnicos aplicables.

El sistema debe reutilizar los componentes existentes en lugar de crear procesos paralelos innecesariamente.

---

# 4. DESCUBRIMIENTO DE DEMANDA

Cuando las páginas que debe contener la web no estén completamente determinadas, debe utilizarse:

`DESCUBRIMIENTO-DEMANDA-E-INTENCIONES.md`

El proceso será:

DEMANDA
↓
KEYWORDS
↓
INTENCIONES
↓
AGRUPACIÓN
↓
OPORTUNIDADES
↓
PRIORIZACIÓN
↓
TIPO DE PÁGINA
↓
ARQUITECTURA
↓
URL

Una keyword no debe convertirse automáticamente en una URL.

La decisión debe basarse en la intención y en la necesidad que existe detrás de la búsqueda.

---

# 5. INVESTIGACIÓN DE KEYWORDS

La investigación debe utilizar datos reales siempre que sea posible.

Pueden utilizarse:

- Google Keyword Planner;
- Google Search Console;
- Google Trends;
- resultados de búsqueda;
- sugerencias de Google;
- búsquedas relacionadas;
- People Also Ask;
- herramientas de keyword research;
- marketplaces;
- foros;
- Reddit;
- comunidades;
- redes sociales;
- consultas de usuarios;
- competidores;
- otras fuentes relevantes.

Cuando una herramienta no esté disponible directamente, el sistema debe poder solicitar al usuario que obtenga y aporte los datos.

Nunca deben inventarse:

- volúmenes;
- CPC;
- dificultad;
- competencia;
- tendencias;
- tráfico;
- conversiones;
- ingresos;
- cualquier otra métrica.

Los datos estimados deben identificarse como estimaciones.

---

# 6. INTENCIÓN DE BÚSQUEDA

La keyword debe interpretarse según lo que realmente quiere conseguir el usuario.

Tipos habituales:

- informacional;
- comercial;
- comparativa;
- transaccional;
- local;
- navegacional;
- resolución de problemas;
- descubrimiento;
- planificación;
- selección;
- preparación;
- ejecución.

El sistema debe crear categorías adicionales cuando sea necesario.

---

# 7. EJEMPLO DE INTERPRETACIÓN

Keyword:

`huerto balcón pequeño`

No debe interpretarse simplemente como:

"crear un artículo sobre huertos".

Puede contener varias necesidades:

- saber qué se puede cultivar;
- saber qué materiales necesita;
- saber cuánto espacio hace falta;
- saber qué productos comprar;
- saber cómo organizar el balcón;
- evitar errores;
- encontrar un kit completo.

Por tanto, primero se debe descubrir la necesidad.

Después se decide qué página o páginas deben existir.

---

# 8. AGRUPACIÓN DE KEYWORDS

Las keywords deben agruparse principalmente por intención.

No por similitud textual.

Ejemplo:

- huerto en balcón;
- huerto balcón pequeño;
- montar huerto en balcón;
- huerto para principiantes en balcón.

Podrían representar una misma intención.

En cambio:

- qué plantar en un balcón;
- cómo regar un huerto de balcón;
- mejores plantas para balcón con sombra.

Pueden representar necesidades diferentes.

La agrupación debe considerar:

- objetivo del usuario;
- solución esperada;
- resultados de búsqueda;
- contenido necesario;
- posibilidad de responder varias consultas con una única página.

---

# 9. VALIDACIÓN MEDIANTE SERP

Cuando sea posible, debe analizarse la página de resultados de búsqueda.

Comprobar:

- qué tipo de páginas aparecen;
- qué necesidades responden;
- qué formato utilizan;
- qué temas cubren;
- si las consultas comparten resultados;
- si existe intención comercial;
- si existe intención transaccional;
- si existen comparativas;
- si existen guías;
- si existen páginas de productos;
- si existen oportunidades desatendidas.

La SERP debe utilizarse como evidencia para decidir si varias keywords pertenecen a una misma intención.

---

# 10. DECISIÓN DE CREAR UNA URL

Una intención puede justificar una URL independiente cuando:

- existe una necesidad claramente diferenciada;
- el usuario espera una respuesta diferente;
- requiere una solución diferente;
- la página puede aportar valor propio;
- existe una razón lógica para que el usuario llegue directamente a ella.

No debe crearse una URL únicamente porque:

- existe una keyword;
- tiene volumen;
- contiene un sinónimo;
- cambia ligeramente la frase;
- cambia una preposición;
- es una variación artificial.

---

# 11. CONSOLIDACIÓN

Antes de crear una URL debe realizarse la siguiente pregunta:

"¿Esta página resuelve una necesidad diferente o puedo resolver correctamente esta necesidad dentro de otra página?"

Si puede resolverse correctamente dentro de otra página:

NO CREAR NUEVA URL.

Si existe una necesidad diferenciada:

PROPONER / CREAR NUEVA URL.

---

# 12. CANIBALIZACIÓN

El sistema debe detectar:

- intenciones iguales;
- intenciones demasiado similares;
- páginas que compiten por la misma búsqueda;
- contenidos duplicados;
- variaciones artificiales;
- páginas que deberían fusionarse.

Las posibles soluciones son:

- fusionar;
- redirigir;
- eliminar;
- cambiar intención;
- diferenciar contenido;
- mantener ambas cuando exista una justificación real.

---

# 13. TIPOS DE PÁGINAS DE AFILIACIÓN

Una web de afiliación puede utilizar diferentes tipos de páginas.

### GUÍA

Resuelve una necesidad mediante información práctica.

Ejemplo:

"Qué necesito para montar un huerto en un balcón"

Puede incluir:

- explicación;
- pasos;
- checklist;
- productos recomendados;
- alternativas;
- presupuesto.

---

### LISTA / KIT

Agrupa productos necesarios para conseguir un objetivo.

Ejemplo:

"Kit para empezar un huerto en un balcón"

Puede incluir:

- macetas;
- sustrato;
- semillas;
- herramientas;
- fertilizante;
- sistema de riego.

---

### COMPARATIVA

Ayuda al usuario a elegir entre varias opciones.

Ejemplo:

"Mejores kits de cultivo para balcón"

---

### PRODUCTO

Presenta un producto concreto cuando exista suficiente valor para hacerlo.

---

### CATEGORÍA

Agrupa productos que responden a una necesidad común.

---

### RANKING

Ordena alternativas según criterios relevantes.

---

### CHECKLIST

Resuelve búsquedas del tipo:

"qué necesito para..."

---

### SOLUCIÓN

Resuelve un problema específico y puede recomendar productos como parte de la solución.

---

# 14. GUÍAS + AFILIACIÓN

Las guías son especialmente importantes cuando el usuario no está buscando directamente un producto.

Ejemplo:

"Qué necesito para pescar en un río"

La página puede responder:

1. permisos;
2. equipamiento;
3. ropa;
4. seguridad;
5. accesorios;
6. recomendaciones;
7. checklist final;
8. productos recomendados.

La afiliación debe formar parte natural de la solución.

No debe introducirse artificialmente.

---

# 15. ESTRUCTURA DINÁMICA

No todas las URLs deben utilizar exactamente la misma estructura de contenido.

El sistema debe disponer de plantillas según la intención.

Por ejemplo:

### PLANTILLA GUÍA

- introducción;
- problema;
- solución;
- pasos;
- materiales;
- recomendaciones;
- errores;
- productos;
- checklist;
- preguntas frecuentes.

### PLANTILLA COMPARATIVA

- resumen;
- criterios;
- opciones;
- comparación;
- ventajas;
- desventajas;
- recomendación;
- alternativas;
- preguntas frecuentes.

### PLANTILLA KIT

- objetivo;
- para quién;
- qué incluye;
- productos;
- alternativas;
- presupuesto;
- montaje;
- checklist.

### PLANTILLA LOCAL

- necesidad;
- solución;
- opciones;
- localización;
- criterios;
- recomendaciones.

La plantilla debe seleccionarse según la intención.

---

# 16. SISTEMA DE BLOQUES

Cuando se utilice WordPress, las páginas deben construirse mediante bloques reutilizables siempre que sea posible.

Ejemplos:

- header;
- introducción;
- problema;
- solución;
- imagen;
- grid;
- producto;
- comparativa;
- checklist;
- pasos;
- ventajas;
- desventajas;
- CTA;
- FAQ;
- enlaces relacionados;
- footer.

Los bloques son componentes.

La estructura de una página es la combinación de esos componentes.

Por tanto:

BLOQUES
+
PLANTILLA DE INTENCIÓN
+
DATOS
+
CONTENIDO
=
PÁGINA

---

# 17. SELECCIÓN AUTOMÁTICA DE PLANTILLA

El sistema puede determinar automáticamente la plantilla.

Ejemplo:

INTENCIÓN:
"qué necesito para hacer X"

↓

TIPO:
CHECKLIST / GUÍA

↓

PLANTILLA:
GUÍA + CHECKLIST + PRODUCTOS

Otro ejemplo:

INTENCIÓN:
"mejor X"

↓

TIPO:
COMPARATIVA

↓

PLANTILLA:
COMPARATIVA

Otro ejemplo:

INTENCIÓN:
"comprar X"

↓

TIPO:
TRANSACCIONAL

↓

PLANTILLA:
PÁGINA COMERCIAL

La selección debe basarse en la intención.

---

# 18. PRODUCTOS

Los productos recomendados deben cumplir una función dentro de la solución.

Cada producto puede incluir:

- nombre;
- imagen;
- descripción;
- utilidad;
- características;
- ventajas;
- inconvenientes;
- precio cuando esté disponible;
- alternativa;
- enlace de afiliado;
- fuente;
- fecha de actualización.

No deben presentarse datos que no hayan sido comprobados.

---

# 19. DATOS DINÁMICOS

Cuando se utilicen productos de terceros:

- utilizar APIs cuando estén disponibles;
- utilizar feeds cuando estén disponibles;
- registrar la fuente;
- controlar cambios;
- actualizar precios;
- detectar productos descatalogados;
- detectar enlaces rotos;
- actualizar imágenes cuando sea necesario.

Los datos dinámicos deben separarse del contenido editorial cuando sea posible.

---

# 20. AUTOMATIZACIÓN

La automatización puede encargarse de:

- descubrir oportunidades;
- recopilar keywords;
- procesar datos;
- clasificar intenciones;
- agrupar keywords;
- generar estructuras;
- seleccionar plantillas;
- obtener productos;
- generar borradores;
- crear páginas;
- actualizar datos;
- comprobar enlaces;
- monitorizar resultados;
- generar informes.

La automatización no debe significar publicación ciega.

---

# 21. CONTROL HUMANO

Las decisiones importantes deben poder revisarse.

Especialmente:

- nuevas categorías;
- nuevas URLs;
- cambios de intención;
- eliminación de páginas;
- publicación masiva;
- selección de productos;
- afirmaciones sensibles;
- información legal;
- decisiones estratégicas.

El sistema debe permitir:

AUTOMÁTICO

o

REVISIÓN HUMANA

según el nivel de riesgo.

---

# 22. ARQUITECTURA RECOMENDADA

Cuando se utilicen WordPress y n8n:

FUENTES
↓
N8N
↓
INVESTIGACIÓN
↓
KEYWORDS
↓
INTENCIONES
↓
OPORTUNIDADES
↓
PLANTILLA
↓
CONTENIDO
↓
PRODUCTOS
↓
VALIDACIÓN
↓
WORDPRESS
↓
PUBLICACIÓN
↓
ANALÍTICA
↓
APRENDIZAJE

La arquitectura concreta debe adaptarse al proyecto.

---

# 23. WORDPRESS

Cuando se utilice WordPress:

- mantener una estructura clara;
- utilizar bloques reutilizables;
- evitar plugins innecesarios;
- separar datos y contenido cuando sea posible;
- controlar actualizaciones;
- realizar backups;
- proteger administración;
- optimizar rendimiento;
- controlar indexación;
- comprobar enlaces;
- comprobar responsive;
- comprobar imágenes.

---

# 24. ESCALABILIDAD

La web debe diseñarse para poder crecer sin aumentar proporcionalmente el trabajo manual.

Debe poder ampliarse mediante:

- nuevas intenciones;
- nuevas categorías;
- nuevos clusters;
- nuevos productos;
- nuevas guías;
- nuevas comparativas;
- nuevas soluciones.

Pero:

ESCALABILIDAD ≠ CREACIÓN MASIVA DE PÁGINAS.

Antes de escalar debe comprobarse que el modelo funciona.

---

# 25. MVP

La primera versión debe ser limitada.

No es necesario crear cientos o miles de páginas.

Debe seleccionarse una muestra representativa.

Ejemplo:

- 1 problema;
- 3-5 intenciones;
- 3-10 páginas;
- varios productos;
- diferentes tipos de página.

El objetivo es comprobar:

- si existe demanda;
- si los usuarios llegan;
- si consumen el contenido;
- si hacen clic;
- si convierten;
- si el proceso de creación funciona;
- si la automatización funciona.

---

# 26. VALIDACIÓN DEL MVP

Medir:

- impresiones;
- clics;
- tráfico;
- tiempo de interacción;
- páginas vistas;
- clics de afiliación;
- conversiones;
- ingresos;
- costes;
- errores.

La decisión posterior puede ser:

ESCALAR

OPTIMIZAR

CAMBIAR

REPLANTEAR

CERRAR

---

# 27. SEO

El SEO debe basarse en necesidades reales.

Debe analizarse:

- intención;
- arquitectura;
- enlazado interno;
- contenido;
- indexabilidad;
- rendimiento;
- competencia;
- autoridad;
- experiencia de usuario.

No debe crearse una página independiente para cada pequeña variación de keyword.

---

# 28. ARQUITECTURA SEMÁNTICA

La web debe organizarse mediante relaciones lógicas.

Ejemplo:

TEMA PRINCIPAL
↓
PROBLEMA
↓
SOLUCIONES
↓
TIPOS
↓
PRODUCTOS
↓
COMPARATIVAS

Esto permite crear:

- enlaces internos;
- clusters;
- páginas pilares;
- páginas satélite;
- rutas de navegación.

La arquitectura debe reflejar cómo se relacionan las necesidades del usuario.

---

# 29. ENLAZADO INTERNO

Las páginas deben conectarse cuando exista una relación real.

Ejemplo:

"Huerto en balcón"

↓

"Qué plantar"

↓

"Qué macetas comprar"

↓

"Kit de huerto"

↓

"Mejores sistemas de riego"

El enlazado debe ayudar al usuario a continuar resolviendo su problema.

---

# 30. MONETIZACIÓN

Las posibles fuentes incluyen:

- enlaces de afiliación;
- comisiones por venta;
- leads;
- reservas;
- CPA;
- CPL;
- programas recurrentes;
- publicidad;
- productos propios;
- servicios propios.

La afiliación no debe ser necesariamente la única fuente de ingresos.

---

# 31. PROGRAMAS DE AFILIACIÓN

Antes de construir alrededor de un proveedor debe comprobarse:

- existencia del programa;
- requisitos;
- países disponibles;
- comisiones;
- duración de cookies;
- método de atribución;
- condiciones;
- restricciones publicitarias;
- restricciones de marca;
- disponibilidad del catálogo;
- estabilidad del programa.

No debe asumirse que un programa seguirá disponible indefinidamente.

---

# 32. COSTES

Registrar:

- dominio;
- hosting;
- WordPress;
- plugins;
- APIs;
- automatización;
- IA;
- almacenamiento;
- herramientas SEO;
- herramientas de investigación;
- mantenimiento;
- otros servicios.

Calcular:

COSTE MENSUAL

COSTE ANUAL

COSTE POR PÁGINA

COSTE POR OPORTUNIDAD

cuando sea posible.

---

# 33. MÉTRICAS ECONÓMICAS

Registrar:

- tráfico;
- clics;
- CTR;
- conversiones;
- comisión media;
- ingresos;
- coste;
- beneficio;
- ROI;
- ingresos por página;
- ingresos por intención.

La métrica final no es el tráfico.

Es:

INGRESOS - COSTES

y, cuando corresponda:

BENEFICIO / TIEMPO INVERTIDO

---

# 34. SEARCH CONSOLE

Cuando la web tenga datos propios, Search Console debe utilizarse para descubrir:

- nuevas keywords;
- nuevas intenciones;
- consultas inesperadas;
- oportunidades;
- páginas con impresiones;
- páginas con CTR bajo;
- páginas que necesitan optimización.

Estas consultas deben poder volver al módulo de descubrimiento.

CICLO:

PUBLICAR
↓
MEDIR
↓
DESCUBRIR
↓
ANALIZAR
↓
OPTIMIZAR
↓
AMPLIAR

---

# 35. APRENDIZAJE

El sistema debe aprender de los resultados reales.

Si una clase de intención funciona:

↑ PRIORIDAD

Si una clase de intención no funciona:

↓ PRIORIDAD

Si una plantilla convierte mejor:

↑ USO

Si una plantilla no funciona:

REVISAR

La web debe convertirse progresivamente en un sistema de aprendizaje.

---

# 36. EXPANSIÓN

Una vez validado un cluster puede buscarse:

- nuevas keywords;
- nuevas intenciones;
- nuevas necesidades;
- nuevos productos;
- nuevas comparativas;
- nuevas guías;
- nuevas categorías.

La expansión debe realizarse desde datos y aprendizaje.

No desde la necesidad artificial de aumentar el número de URLs.

---

# 37. MODELO DE ESCALADO

El proceso recomendado es:

INVESTIGAR
↓
VALIDAR
↓
CREAR MVP
↓
PUBLICAR
↓
MEDIR
↓
OPTIMIZAR
↓
VALIDAR MODELO
↓
ESCALAR

No:

INVESTIGAR
↓
CREAR 10.000 URL
↓
ESPERAR

---

# 38. SEGURIDAD

Nunca deben almacenarse públicamente:

- contraseñas;
- API keys;
- tokens;
- credenciales;
- secretos;
- claves de afiliación privadas.

Deben utilizarse mecanismos seguros de almacenamiento.

---

# 39. CUMPLIMIENTO

Antes de publicar deben revisarse las obligaciones aplicables.

Entre otras:

- privacidad;
- cookies;
- condiciones de uso;
- identificación del responsable;
- divulgación de afiliación;
- derechos de autor;
- uso de marcas;
- condiciones de los programas de afiliación.

La información legal debe revisarse según el país y el modelo concreto.

---

# 40. CONTROL DE CALIDAD

Antes de publicar una página:

### DEMANDA

- intención identificada;
- necesidad clara;
- keywords relacionadas;
- oportunidad justificada.

### CONTENIDO

- responde a la intención;
- aporta valor;
- información coherente;
- ausencia de contenido vacío;
- ausencia de duplicación innecesaria.

### PRODUCTOS

- productos relevantes;
- enlaces correctos;
- datos comprobados;
- afiliación correctamente implementada.

### TÉCNICA

- URL correcta;
- responsive;
- imágenes;
- enlaces;
- velocidad razonable;
- indexación;
- navegación.

### NEGOCIO

- monetización;
- tracking;
- costes;
- métricas.

---

# 41. ESTRUCTURA DE UNA OPORTUNIDAD

Cada oportunidad debería poder registrar:

```text
opportunity_id
project_id
primary_intent
secondary_intents
keywords
search_source
country
language
search_volume
search_volume_status
competition
competition_status
commercial_intent
monetization_potential
user_problem
expected_solution
recommended_page_type
recommended_url
parent_topic
cluster
priority
confidence
evidence
status
created_at
updated_at

Los datos desconocidos deben registrarse como:

N/D

Las estimaciones deben identificarse como:

ESTIMACIÓN


---

42. ESTADOS

Una oportunidad puede pasar por:

DESCUBIERTA

↓

EN INVESTIGACIÓN

↓

AGRUPADA

↓

VALIDADA

↓

PRIORIZADA

↓

APROBADA

↓

EN CONSTRUCCIÓN

↓

PUBLICADA

↓

MEDIDA

↓

OPTIMIZACIÓN

↓

CONSOLIDADA

↓

DESCARTADA


---

43. REGLA CONTRA EL CONTENIDO MASIVO

No debe utilizarse la automatización para crear miles de páginas sin una necesidad real.

Antes de crear una página debe existir:

intención;

necesidad;

solución;

valor;

justificación;

posibilidad de mantenimiento.


Si no existe:

NO CREAR.


---

44. REGLA DE UTILIDAD

Una página debe poder responder:

"¿Qué problema concreto del usuario estoy resolviendo?"

Si la respuesta no es clara:

REVISAR.

Si la única razón para crearla es:

"porque existe una keyword"

NO ES SUFICIENTE.


---

45. PRINCIPIO DE LA WEB GRANDE

Una web puede ser grande y tratar múltiples temáticas.

Pero debe existir una lógica que conecte sus contenidos.

La amplitud no debe significar aleatoriedad.

La web debe construirse alrededor de:

NECESIDADES + SOLUCIONES + RELACIONES ENTRE SOLUCIONES

Una web grande puede contener múltiples áreas siempre que cada una tenga una razón clara para existir.


---

46. EJEMPLO DE ESTRUCTURA

Una web podría tener:

HOGAR

huerto en balcón

organización

herramientas

mantenimiento


OCIO

pesca

senderismo

camping

fotografía


APRENDIZAJE

repostería

bricolaje

jardinería


Cada área puede tener:

PROBLEMAS ↓ GUÍAS ↓ CHECKLISTS ↓ KITS ↓ COMPARATIVAS ↓ PRODUCTOS

La estructura final debe depender de la demanda descubierta.


---

47. PRINCIPIO DE INDEPENDENCIA DEL TIPO DE WEB

El descubrimiento de demanda de


