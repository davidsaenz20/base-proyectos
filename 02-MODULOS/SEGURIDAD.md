# MÓDULO SEGURIDAD

## Propósito

Definir la capacidad reutilizable para incorporar seguridad en cualquier proyecto.

## PRINCIPIO

La seguridad debe considerarse desde el diseño, no añadirse únicamente al final.

## ÁREAS

- Autenticación
- Autorización
- Credenciales
- Datos
- Comunicaciones
- Infraestructura
- Dependencias
- Usuarios
- Logs
- Backups

## AUTENTICACIÓN

Definir:

- cómo se identifica al usuario;
- cómo se almacenan las credenciales;
- cómo se gestionan sesiones;
- cómo se recupera el acceso.

## AUTORIZACIÓN

Definir:

- roles;
- permisos;
- recursos protegidos;
- acciones permitidas.

## CREDENCIALES

Nunca almacenar:

- contraseñas;
- API keys;
- tokens;
- secretos

en código público o documentación compartida.

## DATOS

Identificar:

- datos personales;
- datos sensibles;
- datos críticos;
- información que no debe exponerse.

Aplicar el principio de mínimo acceso.

## COMUNICACIONES

Cuando corresponda utilizar:

- HTTPS;
- conexiones cifradas;
- autenticación segura;
- validación de certificados.

## DEPENDENCIAS

Revisar periódicamente:

- software;
- librerías;
- plugins;
- servicios externos.

## BACKUPS

Definir:

- qué se copia;
- frecuencia;
- retención;
- ubicación;
- recuperación.

## INCIDENTES

Ante un incidente:

1. Detectar.
2. Contener.
3. Analizar.
4. Corregir.
5. Validar.
6. Documentar.

## VALIDACIÓN

Comprobar como mínimo:

- accesos;
- permisos;
- exposición de credenciales;
- protección de datos;
- backups;
- dependencias.

## ESTADO

**Estado:** Base inicial

**Versión:** 1.0

