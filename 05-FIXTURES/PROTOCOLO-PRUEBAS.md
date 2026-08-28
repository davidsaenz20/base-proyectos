# PROTOCOLO DE PRUEBAS DE FIXTURES

## Propósito

Definir cómo deben utilizarse los fixtures de BASE-PROYECTOS para comprobar que la metodología, los tipos de proyecto, los módulos y los procesos definidos en la BASE funcionan correctamente.

Un fixture no es un proyecto real.

Es un entorno controlado utilizado para verificar el comportamiento esperado del sistema.

---

## 1. OBJETIVO DE UNA PRUEBA

Una prueba debe responder:

1. ¿Qué queremos comprobar?
2. ¿Qué información recibe el sistema?
3. ¿Qué proceso debe ejecutar?
4. ¿Qué resultado esperamos?
5. ¿Qué resultado indica PASS?
6. ¿Qué resultado indica FAIL?

Una descripción general del proyecto no constituye por sí misma una prueba.

---

## 2. ESTRUCTURA MÍNIMA

Cada fixture verificable debe poder definir:

IDENTIFICACIÓN
OBJETIVO
ENTRADA
CONTEXTO
MÓDULOS
PROCESO ESPERADO
RESULTADO ESPERADO
CRITERIOS PASS
CRITERIOS FAIL
DEPENDENCIAS
RIESGOS
RESULTADO DE LA PRUEBA

---

## 3. ENTRADA

Debe definirse qué recibe el sistema.

Puede ser:

- una petición de usuario;
- una idea de negocio;
- una especificación;
- una necesidad;
- datos estructurados;
- una combinación de módulos;
- una solicitud de modificación;
- un escenario de error.

La entrada debe ser suficientemente concreta para poder repetir la prueba.

---

## 4. CONTEXTO

Definir las condiciones conocidas del caso.

Ejemplo:

Tipo de proyecto: WEB
Módulos: IA + Email + Seguridad
Objetivo: crear una web informativa
Usuario: cliente de empresa ficticia

No deben incluirse datos innecesarios.

---

## 5. PROCESO ESPERADO

Debe describirse qué debería hacer correctamente el sistema.

Ejemplo:

1. Identificar el tipo de proyecto.
2. Seleccionar los módulos necesarios.
3. Comprobar requisitos.
4. Detectar dependencias.
5. Definir arquitectura.
6. Definir validaciones.
7. Producir el resultado.

El proceso debe poder compararse con el comportamiento real.

---

## 6. RESULTADO ESPERADO

Debe definirse qué debe producir el sistema.

Puede ser:

- decisión;
- arquitectura;
- estructura;
- documentación;
- configuración;
- proyecto;
- código;
- páginas;
- datos;
- workflow;
- informe;
- identificación de riesgos.

Debe evitarse utilizar únicamente expresiones subjetivas como:

"debe estar bien"
"debe funcionar"
"debe ser correcto"

Hay que convertirlas en condiciones comprobables.

---

## 7. CRITERIOS PASS

Una prueba es PASS cuando se cumplen todos los criterios obligatorios definidos para ese caso.

Ejemplo:

PASS si:

- identifica correctamente el tipo WEB;
- utiliza el módulo correspondiente;
- no inventa requisitos;
- define arquitectura;
- identifica riesgos;
- produce todos los elementos obligatorios.

---

## 8. CRITERIOS FAIL

Una prueba es FAIL cuando:

- falta un elemento obligatorio;
- se utiliza un módulo incorrecto;
- se contradicen reglas de la BASE;
- se inventan datos;
- se ignoran dependencias;
- se omite una validación obligatoria;
- se produce un resultado incompatible con el tipo de proyecto.

Los fallos deben documentarse.

---

## 9. PRUEBAS POSITIVAS

Deben comprobar que el sistema funciona correctamente cuando la entrada es válida.

Ejemplo:

Entrada válida
↓
Identificación correcta
↓
Arquitectura correcta
↓
Resultado esperado
↓
PASS

---

## 10. PRUEBAS NEGATIVAS

También deben existir pruebas en las que el sistema deba detectar un problema.

Ejemplos:

- falta información crítica;
- existe una dependencia incompatible;
- el modelo de negocio no es viable;
- un módulo requerido no existe;
- existen requisitos contradictorios;
- una integración no está disponible.

En estos casos el resultado correcto puede ser:

NO CONTINUAR

o:

REQUIERE VALIDACIÓN

No debe considerarse un fallo que el sistema rechace correctamente una entrada no válida.

---

## 11. PRUEBAS DE COMBINACIÓN

Los fixtures deben poder comprobar que varios módulos funcionan juntos.

Ejemplo:

WEB
+
IA
+
API
+
BASE DE DATOS
+
AUTOMATIZACIÓN

Debe comprobarse que:

- las responsabilidades están claras;
- no existen contradicciones;
- las dependencias están identificadas;
- la arquitectura es coherente.

---

## 12. PRUEBAS DE TIPO DE PROYECTO

Cada tipo de proyecto importante debe tener al menos un fixture representativo.

Los tipos actuales incluyen:

- WEB;
- WEB DE AFILIACIÓN;
- APP MÓVIL;
- SaaS;
- Ecommerce;
- API / Servicio;
- Automatización;
- Asistente IA;
- Directorio;
- Portal.

Cuando se incorpore un nuevo tipo de proyecto, debe evaluarse si necesita un fixture específico.

No todos los tipos requieren inicialmente el mismo número de pruebas.

---

## 13. PRUEBAS DE MÓDULOS

Los módulos importantes deben poder comprobarse dentro de uno o varios fixtures.

Debe comprobarse:

- identificación;
- selección;
- integración;
- dependencias;
- comportamiento esperado.

Un módulo no debe considerarse validado simplemente porque exista su archivo.

---

## 14. PRUEBA DE CADENA COMPLETA

La prueba más importante es la cadena:

ENTRADA
↓
ANÁLISIS
↓
TIPO DE PROYECTO
↓
MÓDULOS
↓
REQUISITOS
↓
ARQUITECTURA
↓
CONSTRUCCIÓN
↓
VALIDACIÓN
↓
RESULTADO

El objetivo final de BASE-PROYECTOS es que esta cadena pueda ejecutarse de forma coherente.

---

## 15. RESULTADO DE CADA PRUEBA

Cada fixture verificable debe terminar indicando uno de estos estados:

PASS
FAIL
BLOCKED
NOT RUN

### PASS

La prueba cumple todos los criterios obligatorios.

### FAIL

El sistema produce un resultado incorrecto.

### BLOCKED

No puede ejecutarse porque falta una dependencia necesaria.

### NOT RUN

La prueba está definida pero todavía no se ha ejecutado.

---

## 16. REGISTRO DE FALLOS

Cuando una prueba falle debe registrarse:

- fixture;
- prueba;
- fecha;
- problema;
- causa conocida o hipótesis;
- archivo o módulo afectado;
- corrección propuesta;
- nueva prueba necesaria.

No se debe ocultar un fallo simplemente modificando el estado a PASS.

---

## 17. REPETIBILIDAD

Una prueba debe poder repetirse con la misma entrada y obtener un resultado equivalente.

Cuando el resultado dependa de información externa cambiante, debe registrarse:

- fuente;
- fecha;
- versión;
- condición relevante.

---

## 18. NO CONFUNDIR DOCUMENTACIÓN CON VALIDACIÓN

Un documento que diga:

"Comprobar navegación"

no demuestra que la navegación haya sido comprobada.

Un documento de prueba debe especificar:

Entrada
↓
Acción
↓
Resultado esperado
↓
Criterio PASS/FAIL

---

## 19. PRIORIDAD

Las pruebas deben priorizarse según el riesgo.

Orden recomendado:

1. reglas fundamentales de la BASE;
2. identificación de tipos;
3. selección de módulos;
4. dependencias;
5. arquitectura;
6. construcción;
7. validación;
8. casos especiales;
9. optimización.

---

## 20. REGLA FINAL

Un fixture solo demuestra que la BASE funciona cuando puede utilizarse para detectar correctamente:

- qué debe hacerse;
- qué no debe hacerse;
- qué resultado se espera;
- cuándo una prueba pasa;
- cuándo una prueba falla.

La existencia de un fixture no equivale a una prueba superada.

---

## ESTADO

Estado: Base estructurada para validación

Versión: 2.0

Última revisión: 2026-08-28


