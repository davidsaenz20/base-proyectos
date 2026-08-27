# TIPO DE PROYECTO APP MÓVIL

## Propósito

Definir las características, requisitos y metodología habitual para proyectos de aplicaciones móviles.

Este tipo de proyecto permite construir aplicaciones destinadas principalmente a dispositivos móviles, independientemente de la tecnología concreta utilizada.

## OBJETIVO

Crear una aplicación móvil funcional, mantenible, segura, validada y preparada para evolucionar y distribuirse en los canales correspondientes cuando proceda.

## CARACTERÍSTICAS

Una aplicación móvil puede incluir:

- interfaz móvil;
- navegación entre pantallas;
- formularios;
- autenticación;
- perfiles de usuario;
- almacenamiento local;
- bases de datos;
- APIs;
- notificaciones;
- cámara;
- ubicación;
- archivos;
- pagos;
- compras dentro de la aplicación;
- inteligencia artificial;
- automatizaciones;
- integraciones externas;
- funcionamiento offline o parcialmente offline.

No todos son obligatorios.

## TECNOLOGÍA

La tecnología debe elegirse según las necesidades reales del proyecto.

Puede utilizarse, entre otras opciones:

- desarrollo nativo;
- desarrollo multiplataforma;
- tecnologías web empaquetadas;
- servicios backend externos;
- APIs de terceros.

No se debe elegir una tecnología únicamente por preferencia personal si existe una alternativa más adecuada para el proyecto.

## ARQUITECTURA

Debe definirse antes de construir.

Como mínimo:

- aplicación cliente;
- backend, si existe;
- datos;
- APIs e integraciones;
- autenticación;
- almacenamiento local;
- servicios externos;
- despliegue y distribución.

Debe determinarse qué funciones dependen de Internet y cuáles deben funcionar localmente.

## REQUISITOS

Definir:

- funcionales;
- técnicos;
- seguridad;
- rendimiento;
- experiencia de usuario;
- accesibilidad;
- compatibilidad de dispositivos;
- mantenimiento;
- privacidad y tratamiento de datos.

## VALIDACIÓN

Comprobar como mínimo:

- instalación;
- apertura y cierre;
- navegación;
- formularios;
- autenticación;
- integraciones;
- funcionamiento offline cuando corresponda;
- permisos;
- notificaciones cuando existan;
- visualización en distintos tamaños de pantalla;
- rendimiento;
- consumo razonable de recursos;
- seguridad;
- errores;
- recuperación ante fallos.

## DISTRIBUCIÓN

Definir, cuando corresponda:

- plataforma de distribución;
- cuenta de desarrollador;
- firma de la aplicación;
- identificador de aplicación;
- versiones;
- configuración de producción;
- políticas de publicación;
- procedimiento de actualización;
- procedimiento de retirada o recuperación.

## BACKEND Y SERVICIOS

Si la aplicación utiliza backend, debe documentarse:

- API;
- autenticación;
- base de datos;
- almacenamiento;
- secretos;
- permisos;
- logs;
- monitorización;
- backups;
- recuperación.

La aplicación no debe contener secretos sensibles que deban permanecer en el servidor.

## SEGURIDAD Y PRIVACIDAD

Evaluar:

- autenticación;
- autorización;
- almacenamiento de credenciales;
- cifrado;
- comunicaciones seguras;
- permisos del dispositivo;
- datos personales;
- almacenamiento local;
- terceros;
- exposición de APIs;
- gestión de secretos.

Solo deben solicitarse los permisos necesarios para las funciones reales de la aplicación.

## COSTES

Antes de construir debe estimarse:

- desarrollo;
- backend;
- bases de datos;
- APIs;
- servicios externos;
- almacenamiento;
- distribución;
- mantenimiento;
- monitorización;
- actualizaciones;
- costes recurrentes.

No debe asumirse que una aplicación es barata de mantener únicamente porque su desarrollo inicial sea sencillo.

## ESCALABILIDAD

Debe evaluarse:

- número esperado de usuarios;
- tráfico;
- almacenamiento;
- llamadas a APIs;
- costes variables;
- capacidad del backend;
- límites de servicios externos.

La arquitectura debe ser proporcional al tamaño esperado del proyecto.

## MVP

Cuando exista incertidumbre sobre la demanda o el modelo de negocio, debe priorizarse un MVP que permita validar:

- problema;
- usuario;
- propuesta de valor;
- uso real;
- viabilidad técnica;
- costes;
- modelo de negocio.

No debe construirse una aplicación completa antes de validar los elementos esenciales cuando exista una alternativa de validación más barata.

## MÓDULOS HABITUALES

Según las necesidades del proyecto:

- IA;
- APIs;
- base de datos;
- autenticación;
- automatización;
- pagos;
- notificaciones;
- almacenamiento;
- analítica;
- seguridad;
- observabilidad;
- generación de documentos.

Los módulos especializados deben reutilizar los módulos definidos en `02-MODULOS`.

## RIESGOS

Evaluar:

- dependencia tecnológica;
- dependencia de servicios externos;
- seguridad;
- privacidad;
- rendimiento;
- costes;
- mantenimiento;
- compatibilidad;
- políticas de distribución;
- escalabilidad.

## REGLA

La tecnología debe adaptarse al proyecto.

No se debe construir una arquitectura más compleja de lo necesario.

La aplicación debe diseñarse pensando desde el principio en su mantenimiento y evolución.

## ESTADO

**Estado:** Base inicial

**Versión:** 1.0


