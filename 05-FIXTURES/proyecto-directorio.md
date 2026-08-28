# FIXTURE PROYECTO DIRECTORIO

## Identificación

**Nombre:** Directorio de ejemplo

**Tipo:** Directorio

**Versión:** 2.0

**Estado de la prueba:** NOT RUN

---

## Objetivo

Comprobar que BASE-PROYECTOS puede analizar correctamente un proyecto de tipo Directorio, identificar sus necesidades principales, seleccionar los módulos adecuados, detectar dependencias y riesgos, y producir una estructura de proyecto coherente.

Este fixture es un entorno controlado de prueba.

No representa un directorio real.

---

## Entrada

Crear un directorio digital de profesionales y servicios para una provincia determinada.

El usuario debe poder:

1. buscar un servicio;
2. seleccionar o indicar una localidad;
3. consultar resultados;
4. acceder a una ficha profesional;
5. contactar con el profesional.

### Datos de entrada controlados

**Tipo de proyecto:** Directorio

**Usuarios:** personas que buscan profesionales o servicios.

**Contenido principal:** profesionales, servicios y localidades.

**Resultado solicitado:** definición estructurada del proyecto y de los elementos necesarios para su construcción y validación.

---

## Contexto

El proyecto debe organizar información de profesionales y servicios mediante categorías, localidades y fichas individuales.

La información puede proceder de diferentes fuentes y debe poder mantenerse actualizada.

El sistema debe contemplar:

- búsqueda;
- filtros;
- categorías;
- localidades;
- fichas;
- contacto;
- gestión de datos;
- seguridad;
- mantenimiento;
- escalabilidad.

No se presupone una tecnología concreta.

La arquitectura debe determinarse a partir de los requisitos reales.

---

## Problema

La información sobre profesionales y servicios está dispersa.

El usuario necesita encontrar rápidamente opciones relevantes según:

- servicio;
- localidad;
- categoría;
- características del profesional.

El sistema debe reducir la dificultad de localizar y consultar esa información.

---

## Usuario

Personas que buscan un servicio o profesional.

También puede existir un segundo tipo de usuario:

Profesionales que necesitan gestionar o publicar su información dentro del directorio.

La existencia de funcionalidades específicas para profesionales deberá determinarse durante el análisis del proyecto.

---

## Propuesta

Una plataforma organizada mediante:

- categorías;
- servicios;
- localidades;
- profesionales;
- fichas;
- búsqueda;
- filtros;
- contacto.

La propuesta debe mantenerse dentro del alcance definido por la entrada y no incorporar funcionalidades no justificadas.

---

## Módulos

Módulos potencialmente implicados:

- Directorio
- Web
- Base de datos
- APIs
- Automatización
- Seguridad
- Observabilidad

La prueba debe comprobar que BASE-PROYECTOS:

1. identifica los módulos necesarios;
2. diferencia los módulos necesarios de los opcionales;
3. identifica sus dependencias;
4. evita incorporar módulos sin justificación.

---

## Estructura de datos

Una ficha profesional puede contener:

- identificador;
- nombre;
- servicio;
- categoría;
- localidad;
- descripción;
- datos de contacto;
- estado;
- fecha de actualización.

Los campos definitivos deben determinarse durante el análisis.

No deben inventarse datos reales.

---

## Proceso esperado

### Paso 1. Identificación

Identificar el proyecto como:

**Tipo: Directorio**

### Paso 2. Análisis

Analizar:

- objetivo;
- usuarios;
- contenido;
- búsqueda;
- filtros;
- fichas;
- contacto;
- datos;
- mantenimiento.

### Paso 3. Requisitos

Determinar los requisitos funcionales y no funcionales necesarios.

### Paso 4. Módulos

Seleccionar los módulos correspondientes y justificar su utilización.

### Paso 5. Dependencias

Identificar dependencias entre:

- datos;
- base de datos;
- búsqueda;
- web;
- APIs;
- automatizaciones;
- seguridad;
- observabilidad.

### Paso 6. Arquitectura

Definir una arquitectura coherente con los requisitos.

No debe establecerse una tecnología concreta sin justificación.

### Paso 7. Construcción

Definir los elementos necesarios para construir el proyecto.

### Paso 8. Validación

Definir las pruebas necesarias para comprobar:

- búsqueda;
- filtros;
- resultados;
- fichas;
- contacto;
- navegación;
- datos;
- seguridad;
- comportamiento móvil.

### Paso 9. Resultado

Producir una definición estructurada del proyecto que permita continuar con las siguientes fases de BASE-PROYECTOS.

---

## Resultado esperado

La ejecución correcta debe producir como mínimo:

1. identificación del tipo Directorio;
2. objetivo definido;
3. usuarios identificados;
4. requisitos principales;
5. módulos necesarios;
6. dependencias;
7. riesgos;
8. arquitectura propuesta;
9. proceso de construcción;
10. validaciones;
11. criterios PASS/FAIL;
12. estado final de la prueba.

El resultado debe ser coherente con la información de entrada.

---

## Criterios PASS

La prueba será PASS si:

- identifica correctamente el tipo Directorio;
- mantiene el alcance del proyecto;
- identifica correctamente las necesidades principales;
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
- omite necesidades fundamentales del directorio;
- utiliza módulos sin justificación;
- ignora dependencias importantes;
- ignora riesgos relevantes;
- propone una arquitectura incompatible con los requisitos;
- omite la validación;
- utiliza criterios subjetivos sin condiciones comprobables;
- inventa información no proporcionada;
- no produce alguno de los elementos obligatorios;
- contradice reglas de BASE-PROYECTOS.

---

## Pruebas positivas

### PRUEBA POSITIVA 01 — Directorio básico

**Entrada:**

Directorio de profesionales y servicios organizado por categorías y localidades.

**Resultado esperado:**

Identificación correcta como Directorio y definición de una estructura básica de búsqueda, resultados, fichas y contacto.

**PASS si:**

- identifica Directorio;
- identifica usuarios;
- identifica categorías y localidades;
- identifica fichas;
- identifica búsqueda;
- identifica contacto;
- define validación.

**Estado:** NOT RUN

---

## Pruebas negativas

### PRUEBA NEGATIVA 01 — Información insuficiente

**Entrada:**

"Crear un directorio."

**Resultado esperado:**

El sistema debe detectar que falta información suficiente para definir correctamente el proyecto.

Debe solicitar información adicional o marcar los elementos que requieren validación.

**PASS si:**

- no inventa requisitos;
- identifica la información que falta;
- marca el proyecto como pendiente de validación.

**Estado:** NOT RUN

---

### PRUEBA NEGATIVA 02 — Requisitos contradictorios

**Entrada:**

Crear un directorio en el que todos los datos deban ser privados y, simultáneamente, cualquier usuario deba poder consultar públicamente todas las fichas.

**Resultado esperado:**

Detectar la contradicción y solicitar aclaración antes de continuar con una arquitectura definitiva.

**PASS si:**

- identifica la contradicción;
- no la ignora;
- no inventa una solución;
- solicita validación.

**Estado:** NOT RUN

---

## Pruebas de combinación

### COMBINACIÓN 01

Módulos:

- Directorio
- Web
- Base de datos
- API
- Seguridad
- Automatización

**Debe comprobarse:**

- responsabilidades;
- dependencias;
- flujo de datos;
- seguridad;
- coherencia arquitectónica.

**Estado:** NOT RUN

---

## Riesgos

Riesgos que deben evaluarse:

- datos duplicados;
- datos incorrectos;
- datos desactualizados;
- información incompleta;
- crecimiento del número de fichas;
- crecimiento del tráfico;
- búsquedas ineficientes;
- problemas de seguridad;
- mantenimiento de los datos;
- dependencia de fuentes externas;
- problemas de disponibilidad de APIs;
- información de contacto incorrecta.

No todos los riesgos deben considerarse presentes.

Deben evaluarse según el proyecto real.

---

## Dependencias

Posibles dependencias:

- fuente de datos;
- base de datos;
- sistema de búsqueda;
- interfaz web;
- API;
- sistema de contacto;
- autenticación si fuese necesaria;
- automatizaciones;
- monitorización.

Cada dependencia debe validarse antes de considerarla disponible.

---

## Calidad de datos

Debe comprobarse:

- completitud;
- exactitud;
- actualidad;
- duplicados;
- consistencia;
- formato;
- procedencia;
- estado.

Una ficha no debe considerarse válida únicamente porque exista.

---

## Escalabilidad

Debe evaluarse el comportamiento ante el crecimiento de:

- número de profesionales;
- número de localidades;
- número de servicios;
- número de categorías;
- tráfico;
- consultas;
- volumen de datos.

La solución de escalabilidad debe definirse según las necesidades reales.

---

## Seguridad

Debe evaluarse:

- protección de datos;
- control de acceso;
- exposición de información de contacto;
- validación de entradas;
- protección de APIs;
- gestión de credenciales;
- registros;
- posibles abusos.

Las medidas definitivas deben determinarse durante el diseño.

---

## Validación funcional

Debe comprobarse como mínimo:

### Búsqueda

Entrada:

Una búsqueda de servicio.

Resultado esperado:

Resultados relevantes.

### Localidad

Entrada:

Una localidad.

Resultado esperado:

Resultados asociados a esa localidad.

### Filtros

Entrada:

Servicio + localidad.

Resultado esperado:

Resultados que cumplen los criterios.

### Ficha

Entrada:

Selección de un profesional.

Resultado esperado:

Ficha correspondiente.

### Contacto

Entrada:

Solicitud de contacto.

Resultado esperado:

Ejecución del mecanismo de contacto definido.

### Navegación móvil

Entrada:

Acceso mediante dispositivo móvil.

Resultado esperado:

La información y las funciones principales son utilizables.

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

No representa un directorio real.

No demuestra por sí mismo que BASE-PROYECTOS funcione correctamente.

Su función es proporcionar un escenario reproducible para comprobar el comportamiento de BASE-PROYECTOS ante un proyecto de tipo Directorio.


