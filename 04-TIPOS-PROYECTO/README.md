# 04 — TIPOS DE PROYECTO

Esta carpeta contiene las definiciones y metodologías específicas de cada categoría de proyecto.

Un tipo de proyecto no es un proyecto concreto.

Define las características habituales de una categoría y sirve como referencia para analizar, diseñar, construir y validar proyectos de ese tipo.

---

## TIPOS DISPONIBLES

Actualmente existen los siguientes tipos:

- `WEB.md` — Web
- `WEB-AFILIACION.md` — Web de afiliación
- `APP-MOVIL.md` — Aplicación móvil
- `SAAS.md` — SaaS
- `ECOMMERCE.md` — Ecommerce
- `API-SERVICIO.md` — API / servicio
- `AUTOMATIZACION.md` — Automatización
- `ASISTENTE-IA.md` — Asistente de IA
- `DIRECTORIO.md` — Directorio
- `DIRECTORIO-LOCAL.md` — Directorio local
- `PORTAL.md` — Portal

La lista puede ampliarse cuando aparezca una categoría que justifique una metodología propia.

---

## FUNCIÓN

Los tipos de proyecto permiten adaptar las reglas universales y los módulos reutilizables a las características concretas de cada categoría.

No sustituyen:

- `01-UNIVERSAL`;
- `02-MODULOS`;
- `03-PLANTILLAS`;
- `06-PROYECTOS`;
- ni otros niveles de la arquitectura.

---

## QUÉ DEBE DEFINIR CADA TIPO

Cuando sea relevante, cada tipo puede establecer:

- objetivo habitual;
- características;
- requisitos frecuentes;
- módulos habituales;
- arquitectura habitual;
- fases relevantes;
- riesgos;
- validaciones específicas;
- decisiones habituales;
- costes relevantes;
- dependencias;
- criterios de escalabilidad;
- plantillas recomendadas.

No todos los tipos necesitan exactamente los mismos apartados.

---

## ESPECIALIZACIONES

Un tipo puede especializar a otro.

Ejemplo:

WEB
 ↓
WEB-AFILIACION

`WEB-AFILIACION.md` añade las reglas específicas del modelo de afiliación sin modificar `WEB.md`.

Del mismo modo, un proyecto puede utilizar más de un tipo cuando resulte necesario, siempre que no existan contradicciones.

---

## RELACIÓN CON LOS MÓDULOS

Los tipos de proyecto indican qué módulos pueden resultar habituales.

Los módulos contienen el conocimiento reutilizable.

Ejemplo:

TIPO DE PROYECTO
       ↓
MÓDULOS NECESARIOS
       ↓
CONFIGURACIÓN DEL PROYECTO

Un módulo no debe duplicarse dentro de cada tipo de proyecto salvo que sea necesario para explicar su aplicación específica.

---

## RELACIÓN CON PLANTILLAS

Los tipos de proyecto pueden recomendar plantillas concretas cuando estas aporten valor.

Ejemplo:

TIPO DE PROYECTO
       ↓
PLANTILLAS RECOMENDADAS
       ↓
CONFIGURACIÓN DEL PROYECTO

Las plantillas contienen estructuras reutilizables.

El tipo de proyecto determina cuáles pueden ser apropiadas para esa categoría.

La información específica de un proyecto real no debe incorporarse a las plantillas generales.

---

## RELACIÓN CON PROYECTOS REALES

Cuando se crea un proyecto nuevo:

1. se identifica el tipo o tipos aplicables;
2. se consulta su metodología;
3. se seleccionan los módulos necesarios;
4. se seleccionan las plantillas apropiadas;
5. se adapta la metodología al caso concreto;
6. se registra la configuración del proyecto.

El proyecto real no debe modificar directamente los documentos generales de esta carpeta para almacenar información específica del cliente.

---

## SELECCIÓN DEL TIPO

El sistema no debe seleccionar un tipo únicamente por coincidencia de palabras.

Debe analizar las características reales del proyecto.

Ejemplo:

Una web empresarial sencilla:

WEB

Una web cuyo objetivo principal sea monetizar mediante afiliación:

WEB
+
WEB-AFILIACION

Una aplicación instalada en dispositivos móviles:

APP-MOVIL

Una plataforma con usuarios, cuentas, lógica propia y servicio recurrente:

SAAS

Si un proyecto no encaja claramente en un tipo existente, debe poder continuar utilizando la metodología universal y los módulos correspondientes.

---

## NO FORZAR CATEGORÍAS

Los tipos son herramientas de clasificación, no restricciones.

No se debe forzar un proyecto dentro de una categoría únicamente porque sea conveniente para la documentación.

Cuando una categoría existente no sea suficiente:

- puede combinarse con otra;
- puede utilizarse una categoría principal y especializaciones;
- puede recurrirse directamente a los módulos;
- puede proponerse un nuevo tipo si existe una necesidad recurrente.

---

## VALIDACIÓN

Los tipos de proyecto deben poder comprobarse mediante fixtures.

Una categoría no se considera validada simplemente porque exista su documento.

Debe existir al menos un caso de prueba cuando la importancia de la categoría lo justifique.

Los fixtures se encuentran en:

05-FIXTURES

y siguen:

05-FIXTURES/PROTOCOLO-PRUEBAS.md

---

## REGLA

La información de esta carpeta debe ser:

- reutilizable;
- específica de la categoría;
- independiente de clientes concretos;
- compatible con `01-UNIVERSAL`;
- compatible con `02-MODULOS`;
- compatible con `03-PLANTILLAS`.

No debe contener:

- credenciales;
- secretos;
- datos privados;
- información exclusiva de un proyecto;
- decisiones que solo sean válidas para un cliente concreto.

---

## PRINCIPIO

La arquitectura general de trabajo es:

01-UNIVERSAL
      ↓
02-MODULOS
      ↓
04-TIPOS-PROYECTO
      ↓
03-PLANTILLAS
      ↓
06-PROYECTOS

Esta representación describe el flujo lógico de utilización, no una dependencia estricta de que una capa deba estar físicamente subordinada a otra.

Los tipos adaptan.

Los módulos especializan.

Las plantillas aceleran.

Los proyectos reales ejecutan.

---

## ESTADO

Estado: Base inicial estructurada

Versión: 2.1

Última revisión: 2026-08-28

