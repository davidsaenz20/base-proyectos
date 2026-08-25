# 02 — MÓDULOS

Esta carpeta contiene módulos reutilizables que aportan capacidades específicas a los proyectos.

Un módulo puede ser tecnológico, funcional o de infraestructura.

## Ejemplos

- Inteligencia artificial;
- WhatsApp;
- N8N;
- APIs;
- bases de datos;
- WordPress;
- autenticación;
- pagos;
- correo electrónico;
- generación de documentos;
- almacenamiento;
- analítica.

## Contenido de un módulo

Cada módulo podrá documentar:

- qué es;
- para qué sirve;
- cuándo utilizarlo;
- cuándo no utilizarlo;
- arquitectura;
- configuración;
- dependencias;
- costes;
- riesgos;
- errores habituales;
- buenas prácticas;
- validaciones;
- decisiones reutilizables.

## Regla fundamental

Un módulo debe ser reutilizable en más de un proyecto.

No debe contener información específica de un cliente o proyecto.

## Separación

El conocimiento general del módulo permanece aquí.

La configuración concreta del módulo dentro de un proyecto pertenece al propio proyecto.

## Versionado

Cuando sea necesario, los módulos podrán tener versiones.

Un proyecto deberá poder identificar qué versión de un módulo está utilizando.

## Principio

Los módulos permiten construir proyectos diferentes combinando capacidades existentes, evitando repetir investigación y documentación innecesariamente.




