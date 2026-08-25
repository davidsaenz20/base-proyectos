00-PROTOCOLO-TRABAJO

Tipo: Protocolo temporal de trabajo
Ámbito: Construcción y reorganización de una base universal para futuros proyectos de IA, automatización y software
Estado: ACTIVO
Carácter: TEMPORAL — eliminar al finalizar esta fase

---

1. OBJETIVO DE ESTE TRABAJO

Construir una base documental universal que permita iniciar futuros proyectos tecnológicos sin empezar desde cero.

La base deberá poder utilizarse para proyectos de diferentes tipos, entre ellos:

- webs;
- webs SEO;
- SaaS;
- aplicaciones web;
- aplicaciones móviles;
- automatizaciones;
- sistemas con N8N;
- asistentes de IA;
- servicios de respuesta mediante WhatsApp;
- integraciones mediante APIs;
- herramientas internas;
- pequeños programas;
- software descargable;
- combinaciones de varias tecnologías.

La base no debe estar diseñada alrededor de un único tipo de proyecto.

---

2. PRINCIPIO DE GENERICIDAD

La documentación universal no debe depender estructuralmente de:

- un servicio concreto;
- una localidad concreta;
- un cliente concreto;
- una empresa concreta;
- un dominio concreto;
- una plantilla concreta;
- un tema de WordPress concreto;
- una tecnología concreta cuando exista una alternativa;
- un proyecto concreto.

Los ejemplos específicos deben identificarse como ejemplos o fixtures y mantenerse separados del núcleo universal.

---

3. ESTRUCTURA CONCEPTUAL

Todo el conocimiento deberá clasificarse en cuatro niveles:

UNIVERSAL

Conocimiento aplicable a prácticamente cualquier proyecto.

Ejemplos:

- metodología;
- análisis;
- requisitos;
- arquitectura;
- validación;
- testing;
- seguridad;
- documentación;
- despliegue;
- escalabilidad.

MÓDULO

Conocimiento reutilizable asociado a una tecnología o capacidad.

Ejemplos:

- IA;
- N8N;
- WhatsApp;
- APIs;
- WordPress;
- bases de datos;
- aplicaciones móviles;
- automatización;
- SaaS.

PROYECTO

Información específica de un proyecto concreto.

Ejemplos:

- objetivos;
- requisitos;
- arquitectura elegida;
- clientes;
- servicios;
- dominio;
- configuración;
- datos reales.

FIXTURE / EJEMPLO

Datos utilizados únicamente para probar o demostrar el sistema.

No deben convertirse en dependencias del núcleo universal.

---

4. AUDITORÍA DEL REPOSITORIO EXISTENTE

Antes de crear nueva documentación se debe revisar todo el repositorio "archivo-maestro".

No se debe limitar la revisión a:

"proyecto/seo/"

También deben revisarse los archivos y carpetas existentes fuera de esa ubicación.

El objetivo es:

1. recuperar conocimiento ya desarrollado;
2. detectar conocimiento universal;
3. detectar módulos reutilizables;
4. detectar información específica de proyecto;
5. detectar ejemplos;
6. detectar duplicidades;
7. detectar contradicciones;
8. evitar rehacer trabajo ya realizado.

No se debe crear una nueva versión de algo existente sin comprobar primero si ya existe documentación equivalente.

---

5. NO REHACER EL TRABAJO EXISTENTE

La documentación existente contiene decisiones y trabajo realizado anteriormente.

Por tanto:

- no se debe asumir que un archivo antiguo representa necesariamente el estado actual;
- tampoco se debe asumir que está obsoleto sin comprobarlo;
- se debe contrastar con los documentos relacionados;
- cuando existan varias versiones, debe determinarse cuál es la fuente de verdad;
- no se debe eliminar documentación simplemente porque parezca antigua.

La evolución debe hacerse mediante decisiones explícitas y trazables.

---

6. GITHUB

La conexión disponible con GitHub debe considerarse de solo lectura para este trabajo.

No se debe afirmar nunca que un archivo ha sido:

- creado;
- modificado;
- actualizado;
- eliminado;
- movido;

en GitHub si realmente no se ha ejecutado y confirmado esa operación.

Cuando sea necesario crear o modificar un archivo:

1. leer primero el archivo actual;
2. determinar exactamente qué debe cambiar;
3. entregar al usuario el contenido completo del archivo;
4. indicar claramente el nombre y ubicación del archivo;
5. esperar a que el usuario lo copie y modifique manualmente;
6. continuar solamente cuando el usuario confirme que está hecho.

Nunca entregar únicamente fragmentos cuando la intención sea sustituir el contenido de un archivo.

---

7. INTERVENCIÓN DEL USUARIO

El usuario actualmente trabaja principalmente desde el móvil y no siempre dispone de PC.

Por tanto, se debe priorizar el trabajo que pueda realizarse desde el móvil:

- auditoría;
- análisis;
- arquitectura;
- diseño documental;
- definición de contratos;
- modelos de datos;
- planificación;
- fixtures;
- validaciones;
- especificaciones;
- contenidos preparados para copiar y pegar.

Cuando sea necesaria una acción que requiera PC, debe indicarse claramente:

AHORA TE TOCA A TI — NECESITAS PC

No se debe pedir al usuario que utilice un PC si la tarea puede completarse razonablemente desde el móvil.

---

8. FORMA DE TRABAJO

El trabajo será secuencial.

Proceso:

AUDITAR → DECIDIR → DOCUMENTAR → VALIDAR → SIGUIENTE PASO

No se debe avanzar simplemente por avanzar.

Cada nuevo paso debe tener una razón clara.

Cuando exista una contradicción importante:

DETENER → IDENTIFICAR → RESOLVER → DOCUMENTAR → CONTINUAR

---

9. FUENTES DE VERDAD

Antes de tomar una decisión se deben identificar las fuentes de verdad existentes.

No se debe crear una nueva regla que contradiga silenciosamente una decisión anterior.

Cuando una nueva decisión sustituya a otra:

- identificar la decisión anterior;
- explicar brevemente la sustitución;
- actualizar el documento correspondiente;
- evitar mantener dos reglas incompatibles como si ambas fueran válidas.

---

10. REUTILIZACIÓN

Todo conocimiento que pueda servir para futuros proyectos debe diseñarse como reutilizable.

Si una solución se ha creado para un proyecto concreto pero puede generalizarse, debe analizarse si debe convertirse en:

- principio universal;
- módulo reutilizable;
- plantilla;
- patrón;
- procedimiento.

No se debe duplicar innecesariamente la misma metodología en cada proyecto.

---

11. TECNOLOGÍA

La base universal no debe imponer una tecnología concreta.

La elección tecnológica debe realizarse después de analizar:

- problema;
- requisitos;
- usuarios;
- costes;
- complejidad;
- mantenimiento;
- seguridad;
- escalabilidad;
- tiempo de desarrollo.

Cuando una solución web sea suficiente, se priorizará frente a software instalable si resulta más sencilla y rentable.

Esto no significa que WordPress sea obligatorio.

Según el proyecto podrán utilizarse:

- WordPress;
- aplicaciones web;
- SaaS;
- aplicaciones móviles;
- APIs;
- N8N;
- bases de datos;
- IA;
- software de escritorio;
- otras tecnologías;
- combinaciones de ellas.

---

12. PERFIL DEL USUARIO

El usuario:

- no es programador profesional;
- sabe utilizar WordPress;
- tiene conocimientos de HTML;
- tiene conocimientos de CSS;
- puede trabajar con herramientas de automatización;
- está aprendiendo progresivamente tecnologías adicionales.

Las soluciones deben tener esto en cuenta.

No se debe recomendar complejidad técnica innecesaria.

Cuando sea posible, se debe priorizar:

simple → funcional → rentable → mantenible → escalable

---

13. NEGOCIO ANTES QUE TECNOLOGÍA

Una idea tecnológica no debe construirse simplemente porque sea técnicamente posible.

Antes de implementar se debe comprobar:

- problema real;
- usuario;
- necesidad;
- propuesta de valor;
- competencia;
- costes;
- modelo de ingresos;
- viabilidad;
- mantenimiento;
- posibilidad de escalar.

La tecnología debe estar al servicio del negocio.

---

14. DOCUMENTACIÓN BASE

La nueva "BASE-PROYECTOS" deberá construirse utilizando como materia prima todo el conocimiento reutilizable encontrado en "archivo-maestro".

No se debe copiar automáticamente la estructura actual.

Primero debe analizarse.

La nueva base debe ser:

- más genérica;
- más limpia;
- más reutilizable;
- menos dependiente de proyectos concretos;
- compatible con diferentes tecnologías;
- preparada para futuros proyectos.

---

15. SEPARACIÓN DEL PROYECTO SEO

La documentación de:

"proyecto/seo/"

se considera documentación específica del sistema de webs SEO.

Puede aportar conocimiento reutilizable a "BASE-PROYECTOS", pero no debe definir por sí sola la arquitectura universal.

Los conceptos reutilizables deben extraerse y generalizarse.

---

16. REGLA CONTRA LA DERIVA

Si durante el trabajo aparece una idea nueva que no pertenece al paso actual:

- se registra mentalmente como posible mejora;
- no se cambia inmediatamente el objetivo;
- no se abandona el paso actual sin motivo;
- se continúa con el objetivo establecido.

Una mejora interesante no significa automáticamente que haya que cambiar de dirección.

---

17. CONTROL DE CAMBIOS

Antes de proponer un cambio importante se debe comprobar:

- qué documento afecta;
- qué documentos dependen de él;
- qué decisiones anteriores podrían verse afectadas;
- si existen duplicidades;
- si el cambio debe ser universal o específico.

Los cambios estructurales deben hacerse de forma coherente y no mediante modificaciones aisladas.

---

18. FINALIDAD DE ESTE PROTOCOLO

Este archivo existe únicamente para mantener alineado el trabajo durante la construcción de "BASE-PROYECTOS".

No forma parte del conocimiento universal definitivo.

Cuando "BASE-PROYECTOS" esté terminada y las reglas universales hayan sido incorporadas a la documentación permanente correspondiente, este archivo deberá eliminarse.

---

19. REGLA FINAL

Antes de cada avance importante:

REVISAR → COMPROBAR → DECIDIR → EJECUTAR

Nunca:

SUPONER → CREAR → CONTINUAR

El objetivo no es producir muchos archivos.

El objetivo es construir una base documental correcta, reutilizable y coherente que permita desarrollar futuros proyectos sin empezar de cero.
