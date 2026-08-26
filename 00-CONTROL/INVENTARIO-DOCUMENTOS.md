INVENTARIO DE DOCUMENTOS

Objetivo

Mantener un inventario real y actualizado de la documentación existente en BASE-PROYECTOS.

Este documento refleja la estructura documental real del repositorio y sirve como referencia para evitar duplicidades, documentos obsoletos o capas innecesarias.

Regla principal

Crear y mantener el menor número de documentos posible, siempre que se conserve:

- control;
- trazabilidad;
- metodología;
- reutilización;
- capacidad de ejecución;
- validación;
- seguridad;
- evolución del sistema.

El inventario debe reflejar los archivos reales existentes, no una estructura propuesta o futura.

---

00 — CONTROL

Documento| Finalidad
"README.md"| Explicación rápida de la carpeta de control
"OBJETIVO.md"| Objetivo operativo de BASE-PROYECTOS
"ESTADO.md"| Estado actual del sistema
"ROADMAP.md"| Evolución y trabajo pendiente
"DECISIONES.md"| Registro de decisiones importantes
"INVENTARIO-DOCUMENTOS.md"| Inventario de documentación

---

01 — UNIVERSAL

Documento| Finalidad
"README.md"| Explicación de la capa universal
"PRINCIPIOS.md"| Principios generales del sistema
"REGLAS.md"| Reglas generales de trabajo
"METODOLOGIA-UNIVERSAL.md"| Metodología común
"PROTOCOLO-EJECUCION.md"| Protocolo para ejecutar proyectos
"VALIDACION.md"| Sistema de validación
"SEGURIDAD.md"| Reglas generales de seguridad
"RIESGOS.md"| Gestión de riesgos
"DOCUMENTACION.md"| Sistema de documentación
"CAMBIOS.md"| Registro y gestión de cambios
"MEJORAS-SISTEMA.md"| Evolución y mejora del sistema
"BENCHMARK-SISTEMA.md"| Evaluación y comparación del sistema
"BIBLIOTECA-MODOS-TRABAJO.md"| Modo operativo general de trabajo

---

02 — MODULOS

Documento| Finalidad
"README.md"| Explicación de la capa de módulos
"IA.md"| Módulo de inteligencia artificial
"N8N.md"| Módulo de automatización con n8n
"APIS.md"| Integración con APIs
"BASE-DATOS.md"| Bases de datos
"ARCHIVOS.md"| Gestión de archivos
"AUTENTICACION.md"| Autenticación
"AUTOMATIZACION.md"| Automatización
"EMAIL.md"| Email
"NOTIFICACIONES.md"| Notificaciones
"OBSERVABILIDAD.md"| Observabilidad y monitorización
"PAGOS.md"| Pagos
"SEGURIDAD.md"| Seguridad técnica
"WHATSAPP.md"| Integración con WhatsApp
"WORDPRESS.md"| Integración con WordPress
"ANALITICA.md"| Analítica

---

03 — PLANTILLAS

Documento| Finalidad
"README.md"| Explicación de la capa de plantillas
"FLUJO-EJECUCION-PROYECTO.md"| Flujo reutilizable de ejecución
"PLANTILLA-PROYECTO.md"| Estructura base de un proyecto
"PLANTILLA-REQUISITOS.md"| Definición de requisitos
"PLANTILLA-ARQUITECTURA.md"| Arquitectura
"PLANTILLA-DATOS.md"| Estructura de datos
"PLANTILLA-DECISIONES.md"| Registro de decisiones
"PLANTILLA-IMPLEMENTACION.md"| Implementación
"PLANTILLA-ROADMAP.md"| Roadmap
"PLANTILLA-VALIDACION.md"| Validación
"PLANTILLA-TESTING.md"| Testing
"PLANTILLA-MONITORIZACION.md"| Monitorización
"PLANTILLA-DESPLIEGUE.md"| Despliegue
"proyecto.md"| Plantilla/estructura auxiliar de proyecto

---

Criterios de mantenimiento

1. Fuente de verdad

El árbol real del repositorio es la referencia para determinar qué documentos existen.

La memoria conversacional no sustituye a la documentación persistente.

2. No duplicar funciones

Antes de crear un documento nuevo debe comprobarse si otro documento existente puede cumplir esa función.

Si existe solapamiento importante, se debe estudiar la unificación antes de crear otro archivo.

3. No eliminar por apariencia

Un documento no debe eliminarse únicamente porque parezca redundante.

Primero debe comprobarse:

- qué función cumple;
- qué documentos lo utilizan;
- si contiene información única;
- si puede integrarse en otro documento;
- si su eliminación rompe alguna parte del sistema.

4. Documentos nuevos

Todo documento nuevo debe incorporarse al inventario después de su creación.

5. Cambios estructurales

Cuando se modifique la arquitectura documental, debe actualizarse este inventario y registrarse la decisión correspondiente.

6. Auditorías

Durante una auditoría se puede detectar que un documento debe modificarse.

Eso no implica cambiar de metodología: el modo de trabajo permite analizar, decidir, corregir, validar y continuar dentro del mismo proceso.

Estado de este inventario

Este documento debe mantenerse sincronizado con el árbol real de BASE-PROYECTOS.

Última revisión: 2026-08-26


