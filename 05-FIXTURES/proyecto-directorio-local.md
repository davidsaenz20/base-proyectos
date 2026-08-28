# FIXTURE — PRUEBA PROYECTO DIRECTORIO LOCAL

## Identificación

**Nombre:** Directorio Local de Servicios Ejemplo

**Tipo:** DIRECTORIO-LOCAL

**Versión:** 1.0

**Estado de prueba:** NOT RUN

---

## 1. OBJETIVO

Comprobar que BASE-PROYECTOS puede analizar correctamente un proyecto de tipo DIRECTORIO-LOCAL, diferenciándolo de un Directorio genérico y detectando sus necesidades específicas de servicio, localidad, generación de páginas, SEO local, datos y escalabilidad.

Este fixture es ficticio y no representa un proyecto real.

---

## 2. ENTRADA

Crear una plataforma que permita localizar profesionales y servicios según una combinación de servicio y localidad.

Ejemplo conceptual:

**Servicio + localidad**

La plataforma debe poder incluir:

- páginas por servicio;
- páginas por localidad;
- combinaciones servicio + localidad;
- fichas profesionales;
- categorías;
- buscador;
- filtros;
- formularios;
- contacto;
- contenido;
- datos estructurados.

---

## 3. CONTEXTO

**Usuario principal:** persona que busca un servicio o profesional en una localidad determinada.

**Usuario secundario:** profesional o empresa que puede aparecer o gestionar información dentro del directorio.

**Objetivo:** conectar una necesidad concreta con un servicio o profesional relevante en una localidad.

**Tipo esperado:** DIRECTORIO-LOCAL.

**Complejidad:** media.

El proyecto puede utilizar generación automatizada de páginas, pero la generación masiva no debe considerarse válida por sí misma.

---

## 4. MÓDULOS PREVISTOS

Módulos potencialmente aplicables:

- Directorio;
- Web;
- Base de datos;
- SEO;
- IA;
- Automatización;
- APIs;
- Seguridad;
- Observabilidad;
- WhatsApp;
- Email.

El sistema debe determinar cuáles son realmente necesarios.

No debe añadir módulos únicamente porque aparezcan en este fixture.

---

## 5. PROCESO ESPERADO

1. Identificar la entrada como DIRECTORIO-LOCAL.
2. Diferenciarlo de un Directorio genérico.
3. Identificar la relación servicio + localidad.
4. Extraer los requisitos funcionales.
5. Determinar la estructura de datos.
6. Determinar los módulos necesarios.
7. Identificar dependencias.
8. Definir la arquitectura.
9. Evaluar la generación de páginas.
10. Evaluar requisitos de SEO local.
11. Identificar riesgos de contenido duplicado y baja calidad.
12. Definir validaciones.
13. Evaluar escalabilidad.
14. Producir una especificación previa a la construcción.

---

## 6. RESULTADO ESPERADO

El análisis debe producir como mínimo:

- tipo identificado como DIRECTORIO-LOCAL;
- objetivo definido;
- usuario definido;
- combinación servicio + localidad identificada;
- estructura de datos;
- requisitos funcionales;
- módulos justificados;
- arquitectura;
- dependencias;
- riesgos;
- criterios de validación;
- estrategia de generación controlada;
- criterios básicos de escalabilidad.

La solución debe priorizar utilidad real sobre generación masiva.

---

## 7. CRITERIOS PASS

La prueba será PASS si:

- identifica correctamente DIRECTORIO-LOCAL;
- reconoce la relación servicio + localidad;
- no lo trata simplemente como un Directorio genérico;
- identifica páginas por localidad cuando correspondan;
- identifica páginas por servicio cuando correspondan;
- identifica fichas profesionales;
- identifica búsqueda y filtros cuando sean necesarios;
- selecciona únicamente módulos justificados;
- identifica dependencias relevantes;
- contempla calidad de datos;
- contempla riesgos de contenido duplicado;
- contempla riesgos de generación masiva;
- propone validación antes de escalar;
- propone arquitectura proporcional;
- define criterios de validación;
- no inventa información crítica.

---

## 8. CRITERIOS FAIL

La prueba será FAIL si:

- clasifica el proyecto únicamente como Directorio sin detectar su especialización local;
- ignora la combinación servicio + localidad;
- genera páginas masivamente sin criterios de validación;
- acepta contenido duplicado como estrategia válida;
- ignora calidad de datos;
- omite riesgos relevantes;
- selecciona módulos sin justificación;
- ignora dependencias importantes;
- no contempla escalabilidad;
- no define validaciones;
- inventa información crítica;
- propone una arquitectura desproporcionada.

---

## 9. PRUEBAS NEGATIVAS

### Caso A — Contenido duplicado

Si el sistema propone crear cientos de páginas cambiando únicamente el nombre de la localidad, debe detectar el riesgo de contenido duplicado y exigir validación de utilidad y calidad.

### Caso B — Datos insuficientes

Si no existen datos fiables sobre profesionales, servicios o localidades, el sistema no debe inventarlos.

Debe solicitar información o marcar REQUIERE VALIDACIÓN.

### Caso C — Generación masiva prematura

Si se solicita generar miles de páginas sin haber validado una unidad servicio + localidad, el sistema debe detectar el riesgo y recomendar validar primero una unidad.

### Caso D — Directorio general

Si desaparece la dimensión local y el proyecto se convierte en un directorio general de profesionales, el sistema debe evaluar si corresponde a DIRECTORIO.

---

## 10. DEPENDENCIAS

Posibles dependencias:

- fuente de datos;
- base de datos;
- sistema de búsqueda;
- CMS;
- WordPress;
- APIs;
- IA;
- automatización;
- hosting;
- dominio;
- sistema de contacto;
- analítica;
- herramientas SEO.

Cada dependencia debe validarse antes de considerarla disponible.

---

## 11. RIESGOS

- contenido duplicado;
- páginas sin utilidad real;
- información falsa;
- datos desactualizados;
- datos duplicados;
- datos incompletos;
- generación masiva sin control;
- problemas de indexación;
- crecimiento excesivo del número de páginas;
- costes de generación;
- mantenimiento;
- dependencia de fuentes externas;
- problemas de rendimiento;
- problemas de seguridad.

---

## 12. VALIDACIÓN FUNCIONAL

Comprobar:

1. Una combinación servicio + localidad puede identificarse correctamente.
2. La página correspondiente puede generarse o definirse.
3. La página contiene información útil.
4. El contenido no es una simple copia de otra localidad.
5. La ficha profesional es accesible cuando corresponde.
6. La búsqueda funciona.
7. Los filtros funcionan.
8. Los enlaces funcionan.
9. El contacto funciona.
10. La versión móvil es utilizable.
11. Los datos utilizados son trazables o verificables.
12. La unidad puede validarse antes de escalar.

---

## 13. RESULTADO DE LA PRUEBA

**Estado:** NOT RUN

**Fecha:** Pendiente.

**Resultado observado:** Pendiente.

**Incidencias:** Pendiente.

**Correcciones necesarias:** Pendiente.

---

## 14. REGLA DEL FIXTURE

Este fixture no demuestra por sí mismo que BASE-PROYECTOS funcione.

Solo se considerará validado cuando se ejecute la prueba y se comprueben sus criterios PASS/FAIL.

---

## ESTADO

**Estado:** Fixture verificable

**Versión:** 1.0
