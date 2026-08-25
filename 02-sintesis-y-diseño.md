ENTRADA 001 — ARQUITECTURA CONCEPTUAL DE BASE-PROYECTOS

Fecha: 25/08/2026

Fase: 2 — Síntesis y diseño

Progreso de la fase: 8 %

---

1. OBJETIVO

Diseñar la arquitectura de "BASE-PROYECTOS" antes de comenzar su construcción.

La arquitectura debe permitir que el repositorio funcione como una base documental reutilizable para diferentes tipos de proyectos, no como documentación específica de webs SEO.

El protocolo de trabajo establece explícitamente que la base debe poder utilizarse para webs, SaaS, aplicaciones, automatizaciones, N8N, asistentes de IA, WhatsApp, APIs, herramientas internas, pequeños programas, software descargable y combinaciones de tecnologías.

---

2. PRINCIPIO ARQUITECTÓNICO CENTRAL

"BASE-PROYECTOS" no será una colección de manuales independientes.

Será un sistema compuesto por:

NÚCLEO UNIVERSAL
        +
MÓDULOS REUTILIZABLES
        +
PLANTILLAS
        +
TIPOS DE PROYECTO
        +
PROYECTOS DERIVADOS
        +
FIXTURES / EJEMPLOS

Cada capa tendrá una responsabilidad distinta.

---

3. CAPA 1 — NÚCLEO UNIVERSAL

Contendrá las reglas que deberían ser válidas independientemente de la tecnología o del tipo de proyecto.

Ejemplos:

- cómo analizar una idea;
- cómo definir el problema;
- cómo investigar;
- cómo definir requisitos;
- cómo tomar decisiones;
- cómo diseñar arquitectura;
- cómo definir datos;
- cómo validar;
- cómo hacer testing;
- cómo gestionar seguridad;
- cómo desplegar;
- cómo monitorizar;
- cómo mantener;
- cómo mejorar.

No contendrá:

- WordPress como obligación;
- N8N como obligación;
- una API concreta;
- un sector concreto;
- un cliente concreto;
- una estructura SEO concreta.

---

4. CAPA 2 — MÓDULOS REUTILIZABLES

Los módulos contendrán conocimiento especializado que puede reutilizarse en distintos proyectos.

Ejemplos iniciales:

IA
N8N
WHATSAPP
APIs
WORDPRESS
BASES DE DATOS
AUTOMATIZACIÓN
APLICACIONES
SAAS
WEB
SEGURIDAD
OBSERVABILIDAD

Un módulo no es un proyecto.

Es una capacidad reutilizable.

Ejemplo:

MÓDULO WHATSAPP
        ↓
puede utilizarse en:
        ↓
asistente IA
soporte
reservas
ventas
notificaciones
automatizaciones

---

5. CAPA 3 — PLANTILLAS

Las plantillas serán documentos preparados para crear rápidamente un proyecto nuevo.

Ejemplos:

PLANTILLA DE PROYECTO
PLANTILLA DE ROADMAP
PLANTILLA DE REQUISITOS
PLANTILLA DE ARQUITECTURA
PLANTILLA DE DECISIONES
PLANTILLA DE DATOS
PLANTILLA DE VALIDACIÓN
PLANTILLA DE DESPLIEGUE
PLANTILLA DE MONITORIZACIÓN

Las plantillas no deben contener información real de ningún proyecto.

Deben contener estructura reutilizable.

---

6. CAPA 4 — TIPOS DE PROYECTO

Debe existir una capa que permita adaptar la metodología universal al tipo de proyecto.

Ejemplos:

WEB
WEB AUTOMÁTICA
AUTOMATIZACIÓN
IA
IA + WHATSAPP
APP
API
SAAS
SOFTWARE
HERRAMIENTA INTERNA
SISTEMA HÍBRIDO

Estos tipos no deben duplicar toda la metodología universal.

Deben indicar:

- qué módulos suelen ser necesarios;
- qué fases son relevantes;
- qué riesgos son habituales;
- qué validaciones son específicas;
- qué decisiones suelen aparecer.

---

7. CAPA 5 — PROYECTO DERIVADO

Cuando se inicia un proyecto real, no se modifica la base universal.

Se crea una instancia independiente.

Conceptualmente:

BASE-PROYECTOS
        ↓
seleccionar tipo
        ↓
seleccionar módulos
        ↓
copiar plantillas
        ↓
crear proyecto
        ↓
rellenar configuración
        ↓
ejecutar roadmap

El proyecto contiene:

- objetivo;
- problema;
- usuario;
- modelo de negocio;
- requisitos;
- decisiones;
- arquitectura;
- configuración;
- datos;
- estado;
- roadmap;
- evidencias;
- resultados.

---

8. CAPA 6 — FIXTURES / EJEMPLOS

Los ejemplos sirven para demostrar cómo utilizar la metodología.

No deben convertirse en dependencias.

Por ejemplo:

fixture-web-seo/
fixture-asistente-whatsapp/
fixture-automatizacion-facturas/

Podrán utilizarse para probar las plantillas y demostrar cómo se inicia un proyecto.

Pero deben estar claramente separados del núcleo.

---

9. ESTRUCTURA CONCEPTUAL PROPUESTA

La arquitectura conceptual inicial será:

BASE-PROYECTOS
│
├── 00-control/
│
├── 01-universal/
│
├── 02-modulos/
│
├── 03-plantillas/
│
├── 04-tipos-proyecto/
│
├── 05-fixtures/
│
└── 06-proyectos/

Esta estructura es conceptual, todavía no definitiva.

No se crearán estas carpetas hasta terminar el diseño.

---

10. FUNCIÓN DE CADA NIVEL

00-control/

Control general del sistema.

Contendrá únicamente aquello necesario para saber:

- qué es "BASE-PROYECTOS";
- cómo utilizarla;
- cuál es su estado;
- cuáles son sus reglas de mantenimiento.

---

01-universal/

El núcleo metodológico.

Aquí estará el conocimiento que debería sobrevivir aunque cambiemos completamente de tecnología.

---

02-modulos/

Capacidades reutilizables.

Ejemplos:

IA
N8N
WHATSAPP
APIs
WORDPRESS
BASES DE DATOS

---

03-plantillas/

Estructuras reutilizables para crear documentación de proyectos.

---

04-tipos-proyecto/

Adaptaciones de la metodología para categorías de proyectos.

No contendrá proyectos concretos.

---

05-fixtures/

Ejemplos y casos de prueba.

---

06-proyectos/

Proyectos reales derivados de la base.

Cada proyecto deberá ser independiente.

---

11. REGLA DE DEPENDENCIAS

La dirección de dependencia debe ser:

UNIVERSAL
   ↓
MÓDULOS
   ↓
PLANTILLAS / TIPOS
   ↓
PROYECTOS

Nunca al contrario.

Un proyecto concreto no puede convertirse accidentalmente en una dependencia del núcleo universal.

---

12. REGLA DE GENERICIDAD

Antes de introducir un documento en "01-universal/" debemos preguntarnos:

«¿Este documento seguiría siendo válido si mañana el proyecto fuera una aplicación móvil en lugar de una web?»

Si la respuesta es no:

NO → universal

Después se deberá estudiar si pertenece a:

MÓDULO

o:

TIPO DE PROYECTO

o:

PROYECTO

---

13. REGLA DE GENERALIZACIÓN

Cuando encontremos una solución concreta:

PROBLEMA CONCRETO
↓
SOLUCIÓN
↓
¿SE PUEDE GENERALIZAR?

Si sí:

PRINCIPIO UNIVERSAL

o:

MÓDULO

Si no:

PROYECTO

Esta será una de las operaciones fundamentales de la síntesis.

---

14. REGLA CONTRA LA DUPLICACIÓN

No se debe crear:

metodologia-web.md
metodologia-app.md
metodologia-whatsapp.md
metodologia-n8n.md

si todos contienen las mismas reglas generales.

Debe existir:

METODOLOGÍA UNIVERSAL

y después módulos/adaptaciones específicas.

---

15. REGLA DE CONFIGURACIÓN

Crear un nuevo proyecto debe consistir principalmente en:

SELECCIONAR
+
CONFIGURAR
+
COMPLETAR
+
VALIDAR

y no:

COPIAR
+
REESCRIBIR
+
REINVENTAR

Este principio ya estaba identificado en la documentación de la fábrica de webs y es uno de los objetivos principales de la nueva base.

---

16. REGLA DE TECNOLOGÍA

La arquitectura universal no debe decidir anticipadamente:

WordPress
N8N
Python
React
OpenAI
WhatsApp

La tecnología se seleccionará dentro del proyecto concreto después de analizar:

- problema;
- requisitos;
- usuarios;
- costes;
- complejidad;
- mantenimiento;
- seguridad;
- escalabilidad;
- tiempo de desarrollo.

---

17. REGLA DE CAMBIO TECNOLÓGICO

La metodología debe sobrevivir a un cambio tecnológico.

Ejemplo:

WORDPRESS
   ↓
OTRA PLATAFORMA

no debería obligar a reconstruir:

- metodología;
- sistema de decisiones;
- sistema de validación;
- control de proyecto;
- modelo de documentación.

Solo debería cambiar el módulo o implementación tecnológica correspondiente.

---

18. REGLA PARA EL USUARIO

La arquitectura debe ser suficientemente potente para soportar proyectos profesionales, pero suficientemente sencilla para que el usuario pueda trabajar con ella sin ser programador profesional.

Por tanto:

COMPLEJIDAD INTERNA
≠
COMPLEJIDAD PARA EL USUARIO

La base puede tener una arquitectura sólida internamente, pero la utilización práctica debe ser guiada mediante plantillas y pasos claros.

---

19. RESULTADO ESPERADO

Al finalizar "BASE-PROYECTOS", debería ser posible iniciar algo como:

«Automatización de facturas»

y determinar:

TIPO DE PROYECTO
→ AUTOMATIZACIÓN

MÓDULOS
→ IA
→ DOCUMENTOS
→ APIs
→ BASE DE DATOS
→ AUTOMATIZACIÓN

PLANTILLAS
→ PROYECTO
→ REQUISITOS
→ ARQUITECTURA
→ DATOS
→ VALIDACIÓN
→ DESPLIEGUE

ROADMAP
→ generado/adaptado a ese proyecto

Sin modificar el núcleo universal.

Del mismo modo podría iniciarse:

«Asistente IA para WhatsApp»

o:

«Aplicación móvil para clientes»

o:

«Web automática SEO»

utilizando la misma base.

---

20. DECISIÓN DE ESTA ENTRADA

Se establece provisionalmente que "BASE-PROYECTOS" tendrá una arquitectura de:

CONTROL
UNIVERSAL
MÓDULOS
PLANTILLAS
TIPOS DE PROYECTO
FIXTURES
PROYECTOS

La estructura exacta de archivos y nombres todavía no queda cerrada.

Antes de crearla se realizará una segunda comprobación:

«¿Qué documentos concretos necesitamos realmente dentro de cada nivel?»

El objetivo es evitar crear carpetas y archivos innecesarios.

---

21. SIGUIENTE PASO

El siguiente paso será elaborar el:

INVENTARIO DE DOCUMENTOS UNIVERSALES

Para cada documento propuesto se decidirá:

- nombre;
- finalidad;
- nivel;
- dependencia;
- si es obligatorio u opcional;
- si debe ser plantilla;
- si debe ser módulo;
- si puede eliminarse;
- si ya existe equivalente en "archivo-maestro".

Solo después se aprobará la estructura definitiva.

---

ESTADO

AUDITORÍA ARCHIVO-MAESTRO
████████████████████ 100 %

SÍNTESIS
████████████░░░░░░░░ 60 %

ARQUITECTURA
████░░░░░░░░░░░░░░░░ 20 %

CONSTRUCCIÓN
░░░░░░░░░░░░░░░░░░░░ 0 %

Progreso de la FASE 2: 8 %.

Siguiente paso exacto: inventario de documentos universales.

No tienes que modificar ningún otro archivo ahora. El único trabajo del usuario en este punto es haber añadido esta entrada al "02".


ENTRADA 002 — INVENTARIO MÍNIMO DE DOCUMENTOS DE BASE-PROYECTOS

Fecha: 25/08/2026

Fase: 2 — Síntesis y diseño

Progreso de la fase: 18 %

OBJETIVO

Determinar qué documentación necesita realmente "BASE-PROYECTOS" antes de construirla.

La regla será:

«Crear el menor número de documentos posible, siempre que el sistema conserve control, trazabilidad, reutilización y capacidad de ejecución.»

---

1. NÚCLEO DE CONTROL

Debe existir un único documento principal que explique qué es la base y cómo utilizarla.

README.md

Función:

- explicar el propósito;
- explicar la arquitectura;
- explicar cómo iniciar un proyecto;
- indicar dónde está cada tipo de información.

---

2. METODOLOGÍA UNIVERSAL

Debe existir un documento central:

01-METODOLOGIA-UNIVERSAL.md

Contendrá el método común a cualquier proyecto:

IDEA
↓
INVESTIGACIÓN
↓
DEFINICIÓN
↓
REQUISITOS
↓
DECISIONES
↓
ARQUITECTURA
↓
IMPLEMENTACIÓN
↓
VALIDACIÓN
↓
DESPLIEGUE
↓
OPERACIÓN
↓
MEDICIÓN
↓
MEJORA

---

3. PROTOCOLO UNIVERSAL DE EJECUCIÓN

Debe existir separado de la metodología:

02-PROTOCOLO-EJECUCION.md

Su función será definir cómo se trabaja, no qué proyecto se está construyendo.

Incluirá:

- recuperación de estado;
- paso actual;
- control de alcance;
- bloqueos;
- no desviación;
- documentación;
- validación;
- cierre de pasos;
- reanudación.

---

4. PLANTILLA DE PROYECTO

Debe existir una plantilla que permita iniciar cualquier proyecto:

03-PLANTILLA-PROYECTO.md

Será una estructura vacía para rellenar:

- objetivo;
- problema;
- usuarios;
- propuesta;
- modelo de negocio;
- requisitos;
- restricciones;
- riesgos;
- decisiones;
- arquitectura;
- tecnología;
- módulos;
- estado;
- roadmap.

---

5. PLANTILLA DE ROADMAP

Debe existir:

04-PLANTILLA-ROADMAP.md

No contendrá las fases de una web SEO concreta.

Contendrá una estructura adaptable:

FASE
PASO
OBJETIVO
ENTREGABLE
DEPENDENCIAS
CRITERIO DE FINALIZACIÓN
ESTADO
BLOQUEOS
SIGUIENTE PASO

---

6. PLANTILLA DE DECISIONES

Debe existir:

05-PLANTILLA-DECISIONES.md

Servirá para registrar decisiones importantes:

DECISIÓN
CONTEXTO
ALTERNATIVAS
CRITERIOS
ELECCIÓN
JUSTIFICACIÓN
IMPACTO

La decisión formal no debe depender de la conversación.

---

7. PLANTILLA DE VALIDACIÓN

Debe existir:

06-PLANTILLA-VALIDACION.md

Permitirá definir:

- qué debe funcionar;
- cómo se prueba;
- resultado esperado;
- resultado obtenido;
- evidencia;
- incidencias;
- estado final.

---

8. PLANTILLA DE ESTADO

No necesitamos inicialmente un archivo independiente.

El estado debe formar parte del proyecto y del roadmap.

Debe existir una estructura estándar:

FASE ACTUAL
PASO ACTUAL
OBJETIVO
ENTREGABLE
ESTADO
BLOQUEOS
SIGUIENTE PASO

Decisión: no crear un documento independiente de estado salvo que posteriormente resulte necesario.

---

9. MÓDULOS

Los módulos no necesitan crearse todavía.

La arquitectura permitirá añadirlos posteriormente:

modulos/
├── ia/
├── n8n/
├── whatsapp/
├── wordpress/
├── api/
├── base-datos/
└── ...

Solo se creará un módulo cuando exista conocimiento reutilizable suficiente para justificarlo.

---

10. TIPOS DE PROYECTO

Tampoco se crearán inicialmente muchos tipos.

Primero se definirá una plantilla genérica.

Posteriormente podrán aparecer:

tipos-proyecto/
├── web/
├── automatizacion/
├── ia/
├── app/
├── api/
├── saas/
└── ...

---

11. DECISIÓN PRINCIPAL

El núcleo inicial de "BASE-PROYECTOS" tendrá solamente:

README.md

01-METODOLOGIA-UNIVERSAL.md
02-PROTOCOLO-EJECUCION.md
03-PLANTILLA-PROYECTO.md
04-PLANTILLA-ROADMAP.md
05-PLANTILLA-DECISIONES.md
06-PLANTILLA-VALIDACION.md

Los módulos y tipos de proyecto se añadirán progresivamente.

Esto evita construir una estructura enorme antes de demostrar que es necesaria.

---

12. REGLA DE CRECIMIENTO

"BASE-PROYECTOS" debe crecer por necesidad real.

No se creará un documento porque "podría ser útil".

Se creará cuando:

1. exista una necesidad repetida;
2. la información sea reutilizable;
3. pueda separarse claramente del proyecto concreto;
4. mantenerla en otro documento aporte una ventaja real.

---

ESTADO

AUDITORÍA
████████████████████ 100 %

SÍNTESIS
████████████████░░░░ 80 %

ARQUITECTURA
████████░░░░░░░░░░░░ 40 %

CONSTRUCCIÓN
░░░░░░░░░░░░░░░░░░░░ 0 %

Progreso de la FASE 2: 18 %.

Siguiente paso: definir exactamente qué debe contener cada uno de los seis documentos del núcleo y comprobar que no haya duplicidades entre ellos.



ENTRADA 003 — CONTENIDO Y LÍMITES DE LOS DOCUMENTOS DEL NÚCLEO

Fecha: 25/08/2026

Fase: 2 — Síntesis y diseño

Progreso de la fase: 28 %

OBJETIVO

Definir exactamente qué responsabilidad tendrá cada documento del núcleo para evitar duplicaciones y contradicciones.

---

1. README.md

Responsabilidad:

«Explicar el sistema.»

Debe responder:

- qué es "BASE-PROYECTOS";
- para qué sirve;
- cómo se organiza;
- cómo se inicia un proyecto;
- dónde buscar cada información.

No contendrá la metodología completa.

---

2. 01-METODOLOGIA-UNIVERSAL.md

Responsabilidad:

«Definir qué debe hacerse y por qué.»

Contendrá los principios y fases universales del ciclo de vida de un proyecto.

No contendrá instrucciones operativas detalladas de cómo trabajar con el repositorio.

---

3. 02-PROTOCOLO-EJECUCION.md

Responsabilidad:

«Definir cómo se ejecuta el trabajo.»

Contendrá las reglas de trabajo:

- leer el estado antes de continuar;
- identificar el paso actual;
- trabajar solo en el objetivo actual;
- investigar cuando sea necesario;
- registrar decisiones;
- registrar bloqueos;
- validar;
- cerrar el paso;
- continuar.

No contendrá la metodología completa.

---

4. 03-PLANTILLA-PROYECTO.md

Responsabilidad:

«Crear la documentación inicial de un proyecto concreto.»

Será un documento vacío pero estructurado.

No contendrá decisiones predeterminadas sobre tecnología ni negocio.

---

5. 04-PLANTILLA-ROADMAP.md

Responsabilidad:

«Convertir el proyecto definido en una secuencia ejecutable.»

Cada paso deberá poder contener:

FASE
PASO
OBJETIVO
ENTREGABLE
DEPENDENCIAS
CRITERIO DE FINALIZACIÓN
ESTADO
BLOQUEOS
SIGUIENTE PASO

El roadmap será específico para cada proyecto.

---

6. 05-PLANTILLA-DECISIONES.md

Responsabilidad:

«Mantener un registro formal de las decisiones importantes del proyecto.»

Debe permitir conocer:

- qué se decidió;
- por qué;
- qué alternativas se consideraron;
- qué evidencia se utilizó;
- qué impacto tiene;
- si posteriormente se modificó.

---

7. 06-PLANTILLA-VALIDACION.md

Responsabilidad:

«Demostrar que una parte del proyecto funciona realmente.»

Debe diferenciar:

PREVISTO
↓
PROBADO
↓
RESULTADO
↓
EVIDENCIA
↓
VALIDADO / NO VALIDADO

No se considerará completado un proyecto únicamente porque la documentación diga que debería funcionar.

---

8. REGLA DE NO DUPLICACIÓN

Cada información deberá tener una ubicación principal.

Ejemplo:

METODOLOGÍA
→ qué hacer

PROTOCOLO
→ cómo trabajar

PROYECTO
→ qué estamos construyendo

ROADMAP
→ en qué orden

DECISIONES
→ qué hemos decidido

VALIDACIÓN
→ qué hemos demostrado

Si una información aparece en varios documentos, deberá ser una referencia o resumen, no una segunda versión independiente.

---

9. REGLA DE AUTORIDAD

Cuando exista una contradicción:

1. se identifica el documento que debería ser la fuente de autoridad;
2. se corrige la duplicación;
3. nunca se mantienen dos reglas contradictorias.

La base debe tener una única interpretación válida.

---

10. REGLA DE SEPARACIÓN

La documentación deberá mantener esta separación:

MÉTODO
≠
EJECUCIÓN
≠
PROYECTO
≠
TECNOLOGÍA
≠
RESULTADOS

Esto permitirá reutilizar la metodología aunque cambie completamente el proyecto.

---

11. DECISIÓN

Se confirma que los seis documentos iniciales son suficientes como núcleo documental.

No se añadirá otro documento universal hasta demostrar que existe una responsabilidad que no pueda ubicarse correctamente en uno de ellos.

---

ESTADO

AUDITORÍA
████████████████████ 100 %

SÍNTESIS
██████████████████░░ 90 %

ARQUITECTURA
██████████████░░░░░░ 70 %

CONSTRUCCIÓN
░░░░░░░░░░░░░░░░░░░░ 0 %

Progreso Fase 2: 28 %.

Siguiente paso: diseñar el flujo exacto para crear un proyecto nuevo utilizando estas plantillas.



ENTRADA 004 — FLUJO UNIVERSAL PARA CREAR UN NUEVO PROYECTO

Fecha: 25/08/2026

Fase: 2 — Síntesis y diseño

Progreso de la fase: 36 %

---

1. OBJETIVO

Definir cómo se utilizará "BASE-PROYECTOS" cuando aparezca una idea nueva.

La base debe funcionar como un sistema guiado:

IDEA
↓
CLASIFICACIÓN
↓
INVESTIGACIÓN
↓
DEFINICIÓN
↓
SELECCIÓN DE MÓDULOS
↓
ARQUITECTURA
↓
ROADMAP
↓
CONSTRUCCIÓN
↓
VALIDACIÓN
↓
DESPLIEGUE
↓
OPERACIÓN

---

2. PASO 1 — CAPTURAR LA IDEA

Toda nueva iniciativa comienza con una definición inicial, aunque sea incompleta.

Debe registrarse:

- qué se quiere construir;
- qué problema pretende resolver;
- para quién;
- por qué podría ser útil;
- qué resultado se espera.

En esta fase no se decide todavía la tecnología.

---

3. PASO 2 — CLASIFICAR EL PROYECTO

Se determina qué tipo de proyecto es.

Ejemplos:

WEB
AUTOMATIZACIÓN
IA
IA + WHATSAPP
APP
API
SAAS
SOFTWARE
SISTEMA HÍBRIDO

Un proyecto puede pertenecer a más de un tipo.

Ejemplo:

ASISTENTE IA + WHATSAPP + AUTOMATIZACIÓN

---

4. PASO 3 — INVESTIGAR

Antes de construir se investiga:

- problema;
- usuarios;
- competencia;
- viabilidad;
- requisitos;
- costes;
- riesgos;
- alternativas técnicas;
- alternativas de negocio.

La investigación debe producir decisiones documentadas.

---

5. PASO 4 — DEFINIR

Una vez investigado se concreta:

QUÉ
PARA QUIÉN
POR QUÉ
CÓMO
CON QUÉ LIMITACIONES

El resultado es una definición suficientemente clara para diseñar el sistema.

---

6. PASO 5 — SELECCIONAR MÓDULOS

Se seleccionan únicamente los módulos necesarios.

Ejemplo:

Automatización de facturas
        ↓
IA
Documentos
OCR
API
Base de datos
Automatización

No se deben añadir módulos simplemente porque estén disponibles.

---

7. PASO 6 — DISEÑAR LA ARQUITECTURA

La arquitectura se decide después de conocer:

- requisitos;
- restricciones;
- costes;
- riesgos;
- volumen;
- mantenimiento;
- escalabilidad.

Aquí sí se decide la tecnología.

---

8. PASO 7 — CREAR EL ROADMAP

El proyecto pasa de una idea a una secuencia ejecutable.

Cada paso debe tener:

OBJETIVO
ENTREGABLE
DEPENDENCIAS
CRITERIO DE FINALIZACIÓN
ESTADO

---

9. PASO 8 — CONSTRUIR

Se ejecuta el roadmap.

La construcción no debe modificar arbitrariamente las decisiones anteriores.

Si aparece información nueva que obliga a cambiar una decisión:

NUEVA EVIDENCIA
↓
REVISIÓN
↓
DECISIÓN DOCUMENTADA
↓
ACTUALIZACIÓN DEL ROADMAP

---

10. PASO 9 — VALIDAR

No se considera terminado porque se haya construido.

Debe demostrarse que:

REQUISITO
↓
PRUEBA
↓
RESULTADO
↓
EVIDENCIA

cumple los criterios definidos.

---

11. PASO 10 — DESPLEGAR

Solo después de validar se pasa a producción.

El despliegue deberá contemplar, según el proyecto:

- seguridad;
- backups;
- configuración;
- monitorización;
- recuperación;
- control de errores.

---

12. PASO 11 — OPERAR Y MEJORAR

Una vez funcionando:

MEDIR
↓
DETECTAR
↓
PRIORIZAR
↓
MEJORAR
↓
VOLVER A VALIDAR

El proyecto entra en un ciclo continuo.

---

13. REGLA FUNDAMENTAL

"BASE-PROYECTOS" no debe imponer una única forma de construir.

Debe imponer un orden lógico de pensamiento y control.

La tecnología, herramientas y arquitectura se adaptan al problema.

---

14. RESULTADO

El flujo universal queda definido provisionalmente como:

1. IDEA
2. CLASIFICACIÓN
3. INVESTIGACIÓN
4. DEFINICIÓN
5. MÓDULOS
6. ARQUITECTURA
7. ROADMAP
8. CONSTRUCCIÓN
9. VALIDACIÓN
10. DESPLIEGUE
11. OPERACIÓN
12. MEJORA

---

ESTADO

AUDITORÍA
████████████████████ 100 %

SÍNTESIS
██████████████████░░ 90 %

ARQUITECTURA
████████████████░░░░ 80 %

CONSTRUCCIÓN
░░░░░░░░░░░░░░░░░░░░ 0 %

Progreso Fase 2: 36 %.

Siguiente paso: definir qué información mínima debe contener un proyecto antes de poder pasar de investigación a arquitectura.





