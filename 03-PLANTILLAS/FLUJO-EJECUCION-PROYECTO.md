# FLUJO DE EJECUCIÓN DE PROYECTO

## Propósito

Definir el proceso general que debe seguir un proyecto desde su inicio hasta su funcionamiento real en producción.

Este documento sirve como guía de ejecución para la IA y para las personas que participen en el proyecto.

## Principio

No comenzar a construir directamente.

Primero comprender, después diseñar, después construir, probar y finalmente desplegar.

Cada fase debe producir una salida verificable antes de avanzar a la siguiente.

---

# FASE 1 — ENTRADA

## Objetivo

Comprender qué quiere conseguir el usuario.

## Entrada

- necesidad;
- problema;
- idea;
- petición;
- documentación disponible.

## Acciones

1. Leer la petición.
2. Identificar el objetivo.
3. Identificar el problema.
4. Identificar al usuario.
5. Detectar información desconocida.
6. Determinar si el proyecto es viable de definir.

## Salida

Una primera descripción del proyecto.

## Criterio para avanzar

El objetivo debe estar suficientemente claro para comenzar el análisis.

---

# FASE 2 — ANÁLISIS

## Objetivo

Determinar qué necesita realmente el proyecto.

## Acciones

1. Analizar el problema.
2. Identificar usuarios.
3. Identificar entradas.
4. Identificar procesos.
5. Identificar salidas.
6. Identificar integraciones.
7. Identificar datos.
8. Identificar restricciones.
9. Identificar riesgos.
10. Detectar información que falta.

## Regla

Si falta información importante, preguntar antes de tomar decisiones críticas.

## Salida

Análisis inicial validado.

---

# FASE 3 — CLASIFICACIÓN

## Objetivo

Determinar qué tipo de proyecto se está construyendo.

## Acciones

1. Consultar `04-TIPOS-PROYECTO`.
2. Comparar el proyecto con los tipos disponibles.
3. Seleccionar uno o varios tipos cuando corresponda.
4. Consultar el fixture correspondiente como referencia.
5. No copiar contenido ficticio al proyecto real.

## Salida

Tipo o tipos de proyecto identificados.

---

# FASE 4 — DEFINICIÓN

## Objetivo

Convertir la idea en una definición concreta del proyecto.

## Acciones

Completar la plantilla de proyecto con:

- identificación;
- objetivo;
- problema;
- usuario;
- propuesta;
- alcance;
- requisitos;
- módulos;
- tecnología;
- arquitectura inicial;
- datos;
- riesgos;
- decisiones;
- roadmap;
- validación.

## Salida

`definicion.md`

## Criterio para avanzar

El proyecto debe tener un objetivo, alcance y requisitos suficientemente claros.

---

# FASE 5 — SELECCIÓN DE MÓDULOS

## Objetivo

Determinar qué capacidades reutilizables necesita el proyecto.

## Acciones

1. Consultar `02-MODULOS`.
2. Identificar módulos necesarios.
3. Evitar incorporar módulos innecesarios.
4. Detectar capacidades que todavía no estén documentadas.
5. Si falta una capacidad reutilizable, documentarla como módulo antes de continuar.

## Salida

Lista de módulos seleccionados.

---

# FASE 6 — REQUISITOS

## Objetivo

Definir exactamente qué debe hacer el sistema.

## Acciones

Documentar:

### Requisitos funcionales

- 

### Requisitos técnicos

- 

### Requisitos no funcionales

- 

### Integraciones

- 

### Datos

- 

### Seguridad

- 

## Salida

Requisitos completos y verificables.

---

# FASE 7 — ARQUITECTURA

## Objetivo

Diseñar cómo funcionará el sistema.

## Acciones

Definir:

- componentes;
- servicios;
- APIs;
- bases de datos;
- automatizaciones;
- flujo de información;
- autenticación;
- seguridad;
- almacenamiento;
- observabilidad.

## Regla

La arquitectura debe ser suficientemente sencilla para cumplir el objetivo y suficientemente sólida para funcionar en producción.

## Salida

`arquitectura.md`

---

# FASE 8 — PLANIFICACIÓN

## Objetivo

Convertir la arquitectura en un plan de construcción.

## Acciones

1. Dividir el proyecto en fases.
2. Ordenar las tareas.
3. Identificar dependencias.
4. Identificar bloqueos.
5. Definir criterios de finalización.
6. Establecer el siguiente paso concreto.

## Salida

`roadmap.md`

---

# FASE 9 — CONSTRUCCIÓN

## Objetivo

Construir el sistema.

## Acciones

1. Implementar cada componente.
2. Configurar servicios.
3. Crear integraciones.
4. Configurar automatizaciones.
5. Conectar APIs.
6. Configurar datos.
7. Aplicar seguridad.
8. Documentar decisiones importantes.

## Regla

No considerar una tarea terminada únicamente porque se haya creado un archivo o configuración.

Debe comprobarse que funciona.

## Salida

Primera versión funcional.

---

# FASE 10 — PRUEBAS

## Objetivo

Comprobar que el sistema funciona correctamente.

## Acciones

Realizar pruebas:

- funcionales;
- integración;
- seguridad;
- errores;
- rendimiento cuando sea necesario;
- compatibilidad;
- regresión.

Registrar:

- prueba;
- resultado esperado;
- resultado obtenido;
- estado;
- error;
- corrección.

## Salida

Resultados de testing.

---

# FASE 11 — VALIDACIÓN

## Objetivo

Determinar si el proyecto cumple realmente su objetivo.

## Acciones

Comprobar:

1. requisitos;
2. funcionamiento;
3. seguridad;
4. integraciones;
5. experiencia del usuario;
6. costes;
7. estabilidad;
8. criterios de éxito.

## Regla

Una automatización que técnicamente funciona pero no resuelve el problema del usuario no se considera terminada.

## Salida

`validacion.md`

---

# FASE 12 — DESPLIEGUE

## Objetivo

Poner el sistema en funcionamiento real.

## Acciones

Definir:

- entorno de producción;
- dominio;
- servidores;
- credenciales;
- variables de entorno;
- servicios externos;
- copias de seguridad;
- recuperación;
- permisos;
- configuración final.

## Antes de producción

Comprobar:

- configuración;
- seguridad;
- secretos;
- backups;
- monitorización;
- recuperación ante errores.

## Salida

Sistema desplegado.

---

# FASE 13 — VALIDACIÓN EN PRODUCCIÓN

## Objetivo

Comprobar el comportamiento del sistema real.

## Acciones

1. Ejecutar operaciones reales controladas.
2. Comprobar entradas.
3. Comprobar procesamiento.
4. Comprobar salidas.
5. Comprobar errores.
6. Comprobar notificaciones.
7. Comprobar registros.
8. Comprobar recuperación.

## Criterio

No considerar el proyecto terminado hasta comprobar su funcionamiento en el entorno real.

---

# FASE 14 — MONITORIZACIÓN

## Objetivo

Detectar problemas después del despliegue.

## Acciones

Monitorizar:

- disponibilidad;
- errores;
- rendimiento;
- ejecuciones;
- consumo;
- costes;
- integraciones;
- eventos importantes.

## Salida

Sistema monitorizado.

---

# FASE 15 — CIERRE

## Objetivo

Determinar que el proyecto está terminado.

## Criterios

El proyecto puede considerarse terminado cuando:

- el objetivo se cumple;
- los requisitos están validados;
- las pruebas están superadas;
- la seguridad está revisada;
- el sistema está desplegado;
- funciona en producción;
- existe monitorización;
- existen evidencias;
- la documentación está actualizada.

## Estado final

**Estado:** Terminado

**Progreso:** 100 %

---

# REGLAS DE EJECUCIÓN PARA LA IA

La IA debe:

1. Leer primero el protocolo general.
2. Leer la estructura de la base.
3. Consultar los módulos necesarios.
4. Consultar las plantillas necesarias.
5. Consultar el tipo de proyecto.
6. Mantener separada la información del proyecto real.
7. No inventar información que no conozca.
8. Preguntar cuando falten datos críticos.
9. Validar cada fase antes de avanzar.
10. Registrar decisiones importantes.
11. Mantener actualizado el estado.
12. Mantener actualizado el roadmap.
13. No considerar terminado algo que no haya sido probado.
14. No considerar terminado el proyecto hasta validar su funcionamiento real.

# REGLA PRINCIPAL

**Pensar → definir → diseñar → construir → probar → desplegar → validar → monitorizar → cerrar.**


