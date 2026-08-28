# FIXTURE PROYECTO API SERVICIO

## Identificación

**Nombre:** API de ejemplo

**Tipo:** API Servicio

**Versión:** 2.0

**Estado de la prueba:** NOT RUN

---

## Objetivo

Comprobar que BASE-PROYECTOS puede analizar correctamente un proyecto de tipo API Servicio, identificar sus necesidades, seleccionar los módulos adecuados, detectar dependencias y riesgos, y producir una definición coherente del servicio.

Este fixture es un entorno controlado de prueba.

No representa una API real.

---

## Entrada

Crear una API ficticia que permita a otros sistemas:

1. consultar información;
2. enviar información;
3. modificar información;
4. autenticar peticiones;
5. validar datos;
6. gestionar errores;
7. registrar operaciones.

### Datos de entrada controlados

**Tipo de proyecto:** API Servicio

**Usuarios:** aplicaciones y servicios externos autorizados.

**Contenido principal:** endpoints, peticiones, respuestas, datos, autenticación y operaciones.

**Resultado solicitado:** definición estructurada del proyecto y de los elementos necesarios para su construcción y validación.

---

## Contexto

El proyecto debe proporcionar un servicio centralizado para permitir la comunicación entre diferentes aplicaciones.

No se presupone una tecnología concreta.

La arquitectura debe determinarse a partir de los requisitos reales.

---

## Problema

Diferentes aplicaciones necesitan comunicarse con un servicio centralizado de forma controlada, segura y reproducible.

---

## Usuario

Aplicaciones y servicios externos autorizados.

Los permisos y niveles de acceso deberán determinarse durante el análisis.

---

## Propuesta

Una API con:

- endpoints definidos;
- autenticación;
- autorización;
- validación de datos;
- respuestas estructuradas;
- gestión de errores;
- registro de operaciones;
- control de acceso.

La propuesta debe mantenerse dentro del alcance definido por la entrada.

---

## Módulos

Módulos potencialmente implicados:

- API
- Base de datos
- Seguridad
- Observabilidad
- Automatización

La prueba debe comprobar que BASE-PROYECTOS:

1. identifica los módulos necesarios;
2. diferencia los necesarios de los opcionales;
3. identifica dependencias;
4. justifica su utilización;
5. evita incorporar módulos sin justificación.

---

## Flujo esperado

### Paso 1. Identificación

Identificar el proyecto como:

**Tipo: API Servicio**

### Paso 2. Análisis

Analizar:

- objetivo;
- usuarios;
- endpoints;
- datos;
- autenticación;
- autorización;
- errores;
- seguridad;
- observabilidad;
- mantenimiento.

### Paso 3. Requisitos

Determinar los requisitos funcionales y no funcionales necesarios.

### Paso 4. Módulos

Seleccionar los módulos correspondientes y justificar su utilización.

### Paso 5. Dependencias

Identificar dependencias entre:

- API;
- base de datos;
- autenticación;
- autorización;
- servicios externos;
- observabilidad.

### Paso 6. Arquitectura

Definir una arquitectura coherente con los requisitos.

No establecer una tecnología concreta sin justificación.

### Paso 7. Construcción

Definir los elementos necesarios para construir el servicio.

### Paso 8. Validación

Definir las pruebas necesarias para comprobar:

- peticiones correctas;
- datos incorrectos;
- autenticación;
- permisos;
- errores;
- límites;
- respuestas.

### Paso 9. Resultado

Producir una definición estructurada del proyecto que permita continuar con las siguientes fases de BASE-PROYECTOS.

---

## Resultado esperado

La ejecución correcta debe producir como mínimo:

1. identificación del tipo API Servicio;
2. objetivo definido;
3. usuarios identificados;
4. requisitos principales;
5. endpoints necesarios;
6. módulos necesarios;
7. dependencias;
8. riesgos;
9. arquitectura propuesta;
10. proceso de construcción;
11. validaciones;
12. criterios PASS/FAIL;
13. estado final de la prueba.

---

## Criterios PASS

La prueba será PASS si:

- identifica correctamente el tipo API Servicio;
- mantiene el alcance;
- identifica las necesidades principales;
- define correctamente las operaciones;
- selecciona módulos justificados;
- identifica dependencias relevantes;
- identifica riesgos relevantes;
- define una arquitectura coherente;
- define un proceso de construcción;
- define validaciones concretas;
- establece criterios PASS/FAIL;
- no inventa información no proporcionada;
- produce todos los elementos obligatorios del protocolo.

---

## Criterios FAIL

La prueba será FAIL si:

- identifica incorrectamente el tipo de proyecto;
- omite necesidades fundamentales;
- utiliza módulos sin justificación;
- ignora dependencias importantes;
- ignora riesgos relevantes;
- propone una arquitectura incompatible;
- omite la validación;
- utiliza criterios subjetivos sin condiciones comprobables;
- inventa información no proporcionada;
- no produce alguno de los elementos obligatorios;
- contradice reglas de BASE-PROYECTOS.

---

## Pruebas positivas

### PRUEBA POSITIVA 01 — Petición correcta

**Entrada:**

Cliente autorizado realiza una petición válida a un endpoint disponible.

**Resultado esperado:**

La API autentica la petición, valida los datos, procesa la solicitud y devuelve una respuesta estructurada.

**PASS si:**

- autentica correctamente;
- valida los datos;
- procesa la petición;
- devuelve respuesta;
- registra la operación.

**Estado:** NOT RUN

---

## Pruebas negativas

### PRUEBA NEGATIVA 01 — Petición no autenticada

**Entrada:**

Un cliente realiza una petición sin credenciales válidas.

**Resultado esperado:**

La API rechaza la petición.

**PASS si:**

- detecta la falta de autenticación;
- no procesa la operación;
- devuelve un error adecuado;
- registra el intento cuando corresponda.

**Estado:** NOT RUN

---

### PRUEBA NEGATIVA 02 — Datos inválidos

**Entrada:**

Cliente autorizado envía datos que no cumplen las condiciones esperadas.

**Resultado esperado:**

La API rechaza los datos antes de procesarlos.

**PASS si:**

- detecta los datos inválidos;
- no ejecuta la operación;
- devuelve un error adecuado.

**Estado:** NOT RUN

---

### PRUEBA NEGATIVA 03 — Recurso inexistente

**Entrada:**

Petición válida para consultar un recurso inexistente.

**Resultado esperado:**

La API informa correctamente de que el recurso no existe.

**PASS si:**

- no genera un resultado falso;
- devuelve un error adecuado;
- mantiene una respuesta estructurada.

**Estado:** NOT RUN

---

## Pruebas de combinación

### COMBINACIÓN 01

Módulos:

- API
- Base de datos
- Seguridad
- Observabilidad

**Debe comprobarse:**

- responsabilidades;
- dependencias;
- flujo de datos;
- autenticación;
- autorización;
- registro;
- coherencia arquitectónica.

**Estado:** NOT RUN

---

## Riesgos

Riesgos que deben evaluarse:

- acceso no autorizado;
- exposición de datos;
- credenciales comprometidas;
- datos inválidos;
- abuso de endpoints;
- exceso de peticiones;
- errores internos;
- indisponibilidad de servicios externos;
- pérdida o corrupción de datos;
- errores de integración.

No todos los riesgos deben considerarse presentes.

Deben evaluarse según el proyecto real.

---

## Dependencias

Posibles dependencias:

- base de datos;
- sistema de autenticación;
- servicios externos;
- APIs externas;
- sistema de observabilidad;
- sistemas consumidores.

Cada dependencia debe validarse antes de considerarla disponible.

---

## Seguridad

Debe evaluarse:

- autenticación;
- autorización;
- validación de entradas;
- gestión de credenciales;
- control de acceso;
- límites de peticiones;
- protección de datos;
- protección de APIs;
- registros;
- prevención de abusos.

Las medidas definitivas deben determinarse durante el diseño.

---

## Errores

La API debe gestionar correctamente:

- peticiones inválidas;
- recursos inexistentes;
- falta de permisos;
- errores internos;
- servicios externos no disponibles;
- datos incorrectos.

Los errores deben ser controlados y no deben exponer información innecesaria.

---

## Documentación

Debe definirse como mínimo:

- endpoints;
- parámetros;
- respuestas;
- errores;
- autenticación;
- permisos;
- ejemplos.

La documentación definitiva debe corresponder con la implementación real.

---

## Validación funcional

Debe comprobarse como mínimo:

### Petición correcta

**Entrada:**

Petición autenticada con datos válidos.

**Resultado esperado:**

Respuesta correcta y estructurada.

### Autenticación

**Entrada:**

Petición sin credenciales válidas.

**Resultado esperado:**

Petición rechazada.

### Autorización

**Entrada:**

Usuario autenticado sin permisos suficientes.

**Resultado esperado:**

Operación rechazada.

### Validación

**Entrada:**

Datos incorrectos.

**Resultado esperado:**

Petición rechazada antes de procesarse.

### Error

**Entrada:**

Recurso inexistente.

**Resultado esperado:**

Respuesta de error controlada.

### Límites

**Entrada:**

Número excesivo de peticiones.

**Resultado esperado:**

Aplicación del mecanismo de control correspondiente.

### Respuesta

**Entrada:**

Petición válida.

**Resultado esperado:**

Respuesta estructurada y coherente.

---

## Resultado de la prueba

**Estado actual:** NOT RUN

La existencia de este fixture no significa que la prueba haya sido ejecutada.

Los resultados solo podrán cambiar a:

- PASS;
- FAIL;
- BLOCKED;

después de ejecutar y registrar las pruebas correspondientes.

---

## Registro de ejecución

**Fecha:** Pendiente

**Prueba ejecutada:** Pendiente

**Resultado:** NOT RUN

**Problemas detectados:** Pendiente

**Causa:** Pendiente

**Archivo o módulo afectado:** Pendiente

**Corrección propuesta:** Pendiente

**Nueva prueba necesaria:** Pendiente

---

## Repetibilidad

Las pruebas deben poder repetirse utilizando la misma entrada.

Cuando una prueba dependa de información externa cambiante, debe registrarse:

- fuente;
- fecha;
- versión;
- condición relevante.

---

## Estado

**Estado del fixture:** Verificable

**Estado de ejecución:** NOT RUN

**Versión:** 2.0

**Última revisión:** 2026-08-28

---

## Notas

Este archivo es un fixture controlado.

No representa una API real.

No demuestra por sí mismo que BASE-PROYECTOS funcione correctamente.

Su función es proporcionar un escenario reproducible para comprobar el comportamiento de BASE-PROYECTOS ante un proyecto de tipo API Servicio.

