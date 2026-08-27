# 05 — FIXTURES

Esta carpeta contiene ejemplos, casos de prueba y proyectos ficticios utilizados para comprobar que la metodología y las estructuras de `BASE-PROYECTOS` funcionan correctamente.

Los fixtures sirven como entornos controlados para validar el sistema antes de aplicarlo a proyectos reales.

---

## PROTOCOLO

Las pruebas deben seguir:

`05-FIXTURES/PROTOCOLO-PRUEBAS.md`

Un fixture descriptivo no equivale a una prueba validada.

Para considerar un fixture como prueba debe definir como mínimo:

- objetivo;
- entrada;
- contexto;
- proceso esperado;
- resultado esperado;
- criterios PASS;
- criterios FAIL;
- dependencias;
- riesgos;
- resultado de la ejecución.

---

## TIPOS DE FIXTURES

Aquí pueden existir:

- proyectos ficticios;
- pruebas positivas;
- pruebas negativas;
- escenarios de error;
- pruebas de tipos de proyecto;
- pruebas de módulos;
- pruebas de combinación de módulos;
- pruebas de cadena completa;
- ejemplos controlados.

---

## ESTADOS

Cada prueba puede encontrarse en uno de estos estados:

### NOT RUN

La prueba está definida pero todavía no se ha ejecutado.

### PASS

La prueba se ha ejecutado y cumple todos los criterios obligatorios.

### FAIL

La prueba se ha ejecutado y se ha detectado un comportamiento incorrecto.

### BLOCKED

La prueba no puede ejecutarse porque falta una dependencia necesaria.

---

## REGLA

Un fixture no se considera validado por el simple hecho de existir.

Debe ejecutarse y compararse con sus criterios PASS/FAIL.

Los fixtures deben utilizarse para detectar contradicciones, carencias o errores de `BASE-PROYECTOS`.

Cuando una prueba revele un problema de la BASE, primero debe analizarse y corregirse la causa antes de marcar la prueba como PASS.

---

## REGLA DE LOS EJEMPLOS

Los fixtures son ficticios salvo que se indique expresamente lo contrario.

No deben confundirse con proyectos reales.

---

## ESTADO

**Estado:** Base inicial

**Versión:** 2.0


