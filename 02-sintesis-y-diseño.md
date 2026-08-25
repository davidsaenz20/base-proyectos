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



