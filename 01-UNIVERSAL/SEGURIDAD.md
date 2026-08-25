# SEGURIDAD UNIVERSAL

## Propósito

Definir los principios mínimos de seguridad que deben considerarse en cualquier proyecto.

## Credenciales

Las claves API, contraseñas, tokens y secretos:

- nunca deben quedar expuestos públicamente;
- no deben incluirse directamente en código cuando pueda evitarse;
- deben almacenarse utilizando mecanismos seguros;
- deben poder revocarse o sustituirse.

## Accesos

Cada usuario o servicio debe disponer únicamente de los permisos necesarios para realizar su función.

## Datos

Los datos sensibles deben:

- identificarse;
- protegerse;
- almacenarse únicamente cuando sea necesario;
- eliminarse cuando ya no exista una razón para conservarlos.

## Dependencias externas

Todo servicio externo debe considerarse una dependencia y evaluarse según:

- seguridad;
- disponibilidad;
- costes;
- condiciones de uso;
- dependencia del proveedor.

## Copias y recuperación

Los proyectos que manejen información importante deben disponer de mecanismos adecuados para recuperar datos y configuraciones ante errores.

## Validación

Antes del despliegue se deben revisar los riesgos de seguridad relevantes para el proyecto.

## Regla

La seguridad debe incorporarse durante el diseño, no añadirse únicamente al final del desarrollo.



