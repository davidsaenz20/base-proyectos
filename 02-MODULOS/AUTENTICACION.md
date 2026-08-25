# MÓDULO DE AUTENTICACIÓN

## Propósito

Definir el conocimiento reutilizable necesario para identificar y controlar el acceso de usuarios a un sistema.

## Qué es

La autenticación permite comprobar que un usuario es realmente quien afirma ser.

Debe diferenciarse de la autorización:

- autenticación = quién eres;
- autorización = qué puedes hacer.

## Cuándo utilizarlo

Cuando un proyecto necesita:

- cuentas de usuario;
- áreas privadas;
- perfiles;
- permisos;
- información protegida;
- sesiones;
- acceso restringido.

## Cuándo no utilizarlo

No es necesario cuando toda la funcionalidad del sistema puede utilizarse públicamente y no existen datos o acciones que deban estar protegidos.

## Componentes

Puede incluir:

- registro;
- inicio de sesión;
- cierre de sesión;
- recuperación de acceso;
- gestión de sesiones;
- verificación de identidad;
- roles;
- permisos.

## Métodos

Según el proyecto pueden utilizarse:

- usuario y contraseña;
- enlaces mágicos;
- códigos temporales;
- OAuth;
- proveedores externos;
- autenticación multifactor.

La elección debe depender de los requisitos reales.

## Seguridad

Proteger especialmente:

- contraseñas;
- tokens;
- sesiones;
- credenciales;
- datos personales.

Nunca almacenar contraseñas en texto plano.

## Autorización

La autenticación no concede automáticamente acceso a todos los recursos.

Cada operación debe comprobar que el usuario tiene permisos suficientes.

## Sesiones

Definir:

- duración;
- expiración;
- renovación;
- cierre;
- revocación;
- comportamiento ante pérdida de credenciales.

## Recuperación

El sistema debe disponer de un procedimiento seguro para recuperar el acceso.

No debe permitir que una persona obtenga acceso a otra cuenta mediante información fácilmente adivinable.

## Validación

Comprobar:

- registro;
- inicio de sesión;
- credenciales incorrectas;
- recuperación;
- expiración de sesión;
- cierre de sesión;
- permisos;
- acceso no autorizado;
- múltiples sesiones cuando corresponda.

## Riesgos

- robo de credenciales;
- sesiones comprometidas;
- permisos incorrectos;
- exposición de datos;
- recuperación insegura;
- configuración incorrecta.

## Costes

Evaluar el coste de:

- proveedores externos;
- servicios de autenticación;
- envío de emails;
- SMS;
- infraestructura.

## Dependencias

Puede relacionarse con:

- base de datos;
- email;
- APIs;
- seguridad;
- SaaS;
- aplicaciones web;
- aplicaciones móviles.

## Decisiones reutilizables

Documentar aquí cualquier decisión de autenticación que pueda aplicarse a futuros proyectos.

## Estado

**Estado:** Base inicial

**Versión:** 1.0




