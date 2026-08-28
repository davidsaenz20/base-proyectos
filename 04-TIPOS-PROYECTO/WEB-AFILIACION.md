TIPO DE PROYECTO WEB DE AFILIACIÓN

Propósito

Definir la metodología específica para proyectos web cuyo modelo de negocio principal o complementario sea la afiliación.

Este documento especializa el tipo general "WEB.md" utilizando el módulo:

"02-MODULOS/MODULO-AFILIACION-AUTOMATIZADA.md"

No sustituye al tipo general WEB ni al módulo de afiliación.

---

OBJETIVO

Crear una web de afiliación funcional, útil para el usuario, mantenible, medible y preparada para generar ingresos mediante programas de afiliación.

El objetivo no es publicar páginas automáticamente.

El objetivo es construir un activo digital que pueda adquirir tráfico, generar acciones de afiliación y producir ingresos superiores a sus costes.

---

MODELO DE NEGOCIO

Antes de construir debe definirse:

- nicho;
- público objetivo;
- mercado geográfico;
- problema o necesidad;
- propuesta de valor;
- fuente de tráfico;
- modelo de monetización;
- programas de afiliación;
- estructura de costes;
- hipótesis de ingresos.

La existencia de un programa de afiliación no demuestra por sí misma la viabilidad del proyecto.

---

VALIDACIÓN PREVIA

Antes de desarrollar la web completa debe investigarse:

- demanda;
- competencia;
- intención de búsqueda;
- oportunidades de contenido;
- programas de afiliación;
- requisitos de aprobación;
- comisiones;
- catálogo;
- feeds;
- APIs;
- restricciones;
- costes;
- dificultad técnica;
- potencial de automatización.

El proyecto debe recibir una clasificación:

- 🟢 VIABLE;
- 🟡 VIABLE CONDICIONALMENTE;
- 🟠 REQUIERE VALIDACIÓN;
- 🔴 NO VIABLE.

No se debe construir una web completa cuando la hipótesis de negocio todavía sea claramente inviable.

---

ESTRUCTURA WEB

La arquitectura puede incluir:

- página principal;
- categorías;
- subcategorías;
- fichas de producto o servicio;
- comparativas;
- rankings;
- guías;
- artículos;
- páginas informativas;
- páginas geográficas cuando tengan una justificación real;
- páginas legales;
- páginas de contacto;
- buscador;
- filtros;
- otros componentes necesarios.

La estructura debe responder a las necesidades del usuario y no únicamente a la generación masiva de URLs.

---

CONTENIDO

El contenido debe aportar valor real.

Puede incluir:

- análisis;
- comparativas;
- guías;
- explicaciones;
- selección de productos;
- selección de servicios;
- ventajas y desventajas;
- criterios de compra;
- preguntas frecuentes;
- información contextual.

La IA puede ayudar a generar contenido, pero debe existir un proceso de validación.

No se debe publicar automáticamente contenido falso, duplicado, vacío o creado únicamente para manipular buscadores.

---

DATOS DE AFILIACIÓN

Cuando el proyecto utilice catálogos externos:

- utilizar APIs o feeds oficiales cuando estén disponibles;
- normalizar los datos;
- registrar la fuente;
- registrar la fecha de actualización;
- controlar productos o servicios descatalogados;
- controlar precios potencialmente obsoletos;
- actualizar enlaces cuando sea necesario.

Los datos dinámicos deben mantenerse separados del contenido editorial siempre que sea posible.

---

PRODUCTOS Y SERVICIOS

Una web puede trabajar con:

- productos físicos;
- productos digitales;
- servicios;
- reservas;
- leads;
- suscripciones;
- software;
- viajes;
- hoteles;
- vuelos;
- otros modelos de afiliación.

La estructura debe adaptarse al tipo de conversión.

---

SEO

El SEO debe considerarse una posible fuente de tráfico, no una garantía de tráfico.

Debe analizarse:

- intención de búsqueda;
- arquitectura;
- enlazado interno;
- indexabilidad;
- rendimiento;
- contenido;
- autoridad;
- competencia;
- datos estructurados cuando sean apropiados;
- páginas que realmente aporten valor.

No se debe crear una gran cantidad de páginas únicamente para aumentar el número de URLs indexables.

---

AUTOMATIZACIÓN

La automatización debe utilizarse para reducir trabajo repetitivo.

Puede automatizar:

- importación de datos;
- normalización;
- actualización;
- generación de borradores;
- creación de páginas;
- actualización de precios;
- comprobación de enlaces;
- clasificación;
- publicación cuando sea seguro;
- monitorización;
- informes.

Las tareas que puedan producir errores graves deben incluir validaciones antes de la publicación automática.

---

ARQUITECTURA RECOMENDADA

Cuando resulte adecuado:

FUENTES DE AFILIACIÓN
        ↓
       N8N
        ↓
NORMALIZACIÓN
        ↓
BASE DE DATOS / DATASET
        ↓
REGLAS + IA
        ↓
WORDPRESS
        ↓
WEB
        ↓
USUARIO
        ↓
CLIC / CONVERSIÓN
        ↓
COMISIÓN

La arquitectura real debe adaptarse al proyecto.

No es obligatorio utilizar WordPress ni n8n si otra solución resulta más adecuada.

---

WORDPRESS

Cuando se utilice WordPress:

- separar contenido de datos dinámicos;
- utilizar una estructura mantenible;
- evitar dependencias innecesarias de plugins;
- controlar actualizaciones;
- realizar backups;
- proteger administración;
- optimizar rendimiento;
- evitar publicar automáticamente contenido sin validación cuando exista riesgo.

Los componentes visuales deben poder reutilizarse entre páginas.

---

ESCALABILIDAD

Si el proyecto forma parte de una flotilla de webs:

- reutilizar componentes;
- reutilizar workflows;
- reutilizar modelos de datos;
- reutilizar procesos;
- mantener independencia entre proyectos;
- controlar costes por web;
- medir resultados individualmente.

La creación de nuevas webs debe tener un coste marginal bajo.

No se debe escalar una estrategia antes de demostrar que funciona en una muestra pequeña.

---

MODELO FLOTILLA

Cuando una web haya sido validada, puede utilizarse como plantilla conceptual para crear nuevas oportunidades.

El proceso recomendado es:

INVESTIGAR
↓
VALIDAR
↓
MVP
↓
MEDIR
↓
OPTIMIZAR
↓
DECIDIR
↓
ESCALAR O CERRAR

No se debe asumir que todas las webs de una flotilla tendrán el mismo rendimiento.

Cada web debe considerarse una unidad económica medible.

---

MÉTRICAS

Registrar como mínimo cuando sea posible:

- visitas;
- usuarios;
- páginas vistas;
- impresiones;
- clics afiliados;
- CTR;
- conversiones;
- comisión;
- ingresos;
- costes;
- beneficio estimado;
- páginas indexadas;
- tiempo de mantenimiento;
- errores;
- estado de los programas afiliados.

---

COSTES

Calcular:

- dominio;
- hosting;
- WordPress;
- plugins;
- APIs;
- feeds;
- automatización;
- IA;
- almacenamiento;
- mantenimiento;
- otros servicios externos.

Debe calcularse el coste mensual y anual atribuible a cada proyecto.

---

PUNTO DE EQUILIBRIO

Como regla básica:

INGRESOS > COSTES DIRECTOS

Una web que no alcance el punto de equilibrio después de un periodo razonable de validación debe revisarse.

Las posibles decisiones son:

- optimizar;
- cambiar monetización;
- cambiar contenido;
- cambiar estrategia;
- cambiar nicho;
- vender;
- cerrar;
- no renovar.

---

CUMPLIMIENTO

Antes de publicar deben revisarse las obligaciones aplicables al proyecto, incluyendo cuando corresponda:

- identificación del responsable;
- privacidad;
- cookies;
- consentimiento;
- condiciones de uso;
- divulgación de afiliación;
- derechos de terceros;
- uso de marcas;
- condiciones de los programas de afiliación.

No deben copiarse textos legales de terceros sin verificar su adecuación al proyecto.

---

SEGURIDAD

Evaluar:

- WordPress;
- plugins;
- credenciales;
- APIs;
- claves;
- formularios;
- administración;
- backups;
- actualizaciones;
- integraciones externas.

Las claves y secretos nunca deben publicarse en el repositorio ni en el código del frontend.

---

VALIDACIÓN FINAL

Antes de considerar terminada una web:

Negocio

- programa afiliado operativo;
- enlaces correctos;
- modelo de comisión comprobado;
- costes conocidos.

Contenido

- contenido útil;
- ausencia de errores evidentes;
- ausencia de contenido duplicado innecesario;
- datos actualizados.

Técnica

- navegación;
- responsive;
- velocidad razonable;
- formularios;
- enlaces;
- imágenes;
- errores;
- seguridad básica;
- backups.

Afiliación

- enlaces de afiliado;
- tracking;
- atribución cuando corresponda;
- actualización de productos/servicios;
- comprobación de enlaces rotos.

---

REGLA PRINCIPAL

Una web de afiliación no debe medirse por:

- número de páginas;
- número de productos;
- cantidad de automatizaciones;
- cantidad de webs creadas.

Debe medirse por:

valor para el usuario + tráfico cualificado + conversiones + ingresos - costes.

---

RELACIÓN CON OTROS DOCUMENTOS

Este tipo de proyecto utiliza:

- "04-TIPOS-PROYECTO/WEB.md";
- "02-MODULOS/MODULO-AFILIACION-AUTOMATIZADA.md";
- módulos universales aplicables;
- fixtures y pruebas correspondientes;
- documentación del proyecto concreto.

Cuando exista conflicto, debe prevalecer la arquitectura general del sistema y la decisión documentada correspondiente.

---

ESTADO

Estado: Base inicial

Versión: 1.0

