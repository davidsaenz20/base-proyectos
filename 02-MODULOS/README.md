# 02 — MÓDULOS

Esta carpeta contiene módulos reutilizables que aportan capacidades específicas a los proyectos.

Un módulo puede ser tecnológico, funcional o de infraestructura.

Un módulo debe tener una definición propia cuando exista suficiente conocimiento reutilizable como para justificar su documentación independiente.

---

## ESTADO ACTUAL

La carpeta puede contener módulos en diferentes estados de madurez.

Una capacidad mencionada en un tipo de proyecto no debe considerarse automáticamente un módulo documentado.

Estados posibles:

- PROPUESTO
- EN DESARROLLO
- DOCUMENTADO
- VALIDADO
- DEPRECADO

---

## EJEMPLOS DE CAPACIDADES

La BASE puede necesitar módulos relacionados con:

- inteligencia artificial;
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
- analítica;
- SEO;
- observabilidad;
- seguridad;
- notificaciones.

Esta lista representa capacidades que pueden requerir módulos.

No significa que todas tengan actualmente un archivo de módulo propio.

---

## CUÁNDO CREAR UN MÓDULO

Debe crearse un módulo independiente cuando:

1. la capacidad se utilice en más de un proyecto;
2. exista conocimiento específico que convenga reutilizar;
3. tenga decisiones, dependencias o riesgos propios;
4. su documentación pueda mantenerse independientemente de un proyecto concreto.

No debe crearse un módulo únicamente para completar una lista.

---

## CONTENIDO DE UN MÓDULO

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
- decisiones reutilizables;
- compatibilidades;
- limitaciones;
- versión.

No todos los módulos necesitan exactamente los mismos apartados.

---

## REGLA FUNDAMENTAL

Un módulo debe ser reutilizable en más de un proyecto.

No debe contener información específica de un cliente o proyecto.

---

## SEPARACIÓN

El conocimiento general del módulo permanece aquí.

La configuración concreta del módulo dentro de un proyecto pertenece al propio proyecto.

Ejemplo:

MÓDULO
↓
conocimiento reutilizable

PROYECTO
↓
configuración concreta

---

## RELACIÓN CON LOS TIPOS DE PROYECTO

Un tipo de proyecto puede recomendar capacidades o módulos habituales.

Esto no obliga a que cada capacidad tenga inmediatamente un módulo independiente.

Ejemplo:

TIPO: DIRECTORIO LOCAL

Capacidades habituales:
- web
- WordPress
- IA
- N8N
- SEO
- WhatsApp

Cuando una de esas capacidades tenga suficiente conocimiento reutilizable, podrá convertirse en un módulo propio.

---

## RELACIÓN CON LAS PLANTILLAS

Los módulos aportan capacidades.

Las plantillas proporcionan estructuras reutilizables.

No deben confundirse.

MÓDULO
↓
capacidad reutilizable

PLANTILLA
↓
estructura reutilizable

---

## RELACIÓN CON LOS PROYECTOS

El proyecto selecciona los módulos que realmente necesita.

Por tanto:

TIPO DE PROYECTO
↓
MÓDULOS NECESARIOS
↓
CONFIGURACIÓN DEL PROYECTO

No todos los módulos disponibles deben utilizarse en todos los proyectos.

---

## VERSIONADO

Cuando sea necesario, los módulos podrán tener versiones.

Un proyecto deberá poder identificar qué versión de un módulo está utilizando cuando esa versión afecte a su funcionamiento.

---

## VALIDACIÓN

Un módulo no se considera validado simplemente porque exista su archivo.

La validación debe comprobar, cuando corresponda:

- utilidad;
- coherencia;
- integración;
- dependencias;
- riesgos;
- comportamiento esperado;
- compatibilidad con los proyectos que lo utilizan.

---

## PRINCIPIO

Los módulos permiten construir proyectos diferentes combinando capacidades existentes, evitando repetir investigación y documentación innecesariamente.

La BASE debe crear módulos cuando aporten reutilización real, no para aumentar artificialmente el número de archivos.

---

## ESTADO

Estado: Estructura base de módulos

Versión: 2.0

Última revisión: 2026-08-28

