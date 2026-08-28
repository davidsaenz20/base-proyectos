# FIXTURE: PROYECTO APP MÓVIL

## OBJETIVO

Validar que el sistema puede interpretar, estructurar y planificar correctamente un proyecto de aplicación móvil.

El fixture representa una aplicación móvil con:

- usuarios;
- autenticación;
- API;
- almacenamiento;
- notificaciones;
- funcionamiento parcialmente offline;
- integración externa.

---

## ENTRADA

**Tipo de proyecto:** APP-MOVIL

**Nombre:** Gestión de visitas

**Descripción:**

Aplicación móvil para que técnicos registren visitas realizadas a clientes.

La aplicación debe permitir:

- iniciar sesión;
- consultar visitas asignadas;
- consultar los datos del cliente;
- registrar una visita;
- añadir observaciones;
- adjuntar fotografías;
- guardar temporalmente información sin conexión;
- sincronizar los datos cuando vuelva Internet;
- recibir notificaciones de nuevas visitas.

---

## REQUISITOS FUNCIONALES

### RF-01 — Autenticación

El usuario debe poder iniciar sesión mediante credenciales.

### RF-02 — Visitas

El usuario debe poder consultar las visitas asignadas.

### RF-03 — Detalle

El usuario debe poder consultar los datos necesarios del cliente.

### RF-04 — Registro

El usuario debe poder registrar el resultado de una visita.

### RF-05 — Fotografías

El usuario debe poder adjuntar fotografías a una visita.

### RF-06 — Offline

El usuario debe poder registrar información básica sin conexión.

### RF-07 — Sincronización

Los datos pendientes deben sincronizarse cuando vuelva la conexión.

### RF-08 — Notificaciones

El usuario debe poder recibir notificaciones de nuevas visitas.

---

## REQUISITOS TÉCNICOS

La solución debe contemplar:

- aplicación cliente;
- backend;
- API;
- base de datos;
- autenticación;
- almacenamiento local;
- sincronización;
- almacenamiento de imágenes;
- notificaciones;
- gestión de errores;
- monitorización.

---

## SEGURIDAD

Debe contemplarse:

- comunicaciones HTTPS;
- protección de credenciales;
- gestión segura de tokens;
- autorización;
- protección de APIs;
- almacenamiento seguro de datos sensibles;
- gestión de permisos;
- protección de fotografías.

Los secretos del backend no deben almacenarse dentro de la aplicación móvil.

---

## PRIVACIDAD

La aplicación puede tratar:

- datos identificativos;
- datos de clientes;
- fotografías;
- información relacionada con visitas.

Debe determinarse qué datos son necesarios y cómo se almacenan, transmiten y eliminan.

---

## OFFLINE Y SINCRONIZACIÓN

El comportamiento mínimo esperado es:

```text
USUARIO
   ↓
APP
   ↓
¿HAY INTERNET?
   ├── SÍ → API → SERVIDOR
   │
   └── NO → ALMACENAMIENTO LOCAL
                  ↓
            VUELVE INTERNET
                  ↓
              SINCRONIZAR
```

La solución debe contemplar posibles conflictos y errores de sincronización.

---

## ARQUITECTURA ESPERADA

Una solución válida puede seguir conceptualmente:

```text
APP MÓVIL
   ↓
API
   ↓
BACKEND
   ↓
BASE DE DATOS

APP MÓVIL
   ↓
ALMACENAMIENTO LOCAL
   ↓
SINCRONIZACIÓN
   ↓
API
```

La tecnología concreta no debe considerarse obligatoria.

---

## VALIDACIÓN

El sistema debe comprobar como mínimo:

- instalación;
- apertura;
- inicio de sesión;
- navegación;
- consulta de visitas;
- registro de visita;
- fotografías;
- funcionamiento sin conexión;
- recuperación de conexión;
- sincronización;
- notificaciones;
- permisos;
- errores;
- cierre y reapertura;
- seguridad básica.

---

## CASOS DE PRUEBA

### TEST-01

**Caso:** inicio de sesión correcto.

**Resultado esperado:** acceso al área de visitas.

**PASS:** el usuario accede correctamente.

**FAIL:** se produce acceso incorrecto o error inesperado.

---

### TEST-02

**Caso:** consultar visita asignada.

**Resultado esperado:** se muestran los datos disponibles de la visita.

**PASS:** la visita aparece correctamente.

**FAIL:** la información no aparece o es incorrecta.

---

### TEST-03

**Caso:** registrar visita sin conexión.

**Resultado esperado:** la información queda almacenada localmente.

**PASS:** la información permanece disponible para sincronización.

**FAIL:** se pierde la información.

---

### TEST-04

**Caso:** recuperar conexión.

**Resultado esperado:** los datos pendientes se sincronizan.

**PASS:** los datos llegan correctamente al backend.

**FAIL:** se duplican, pierden o corrompen datos.

---

### TEST-05

**Caso:** adjuntar fotografía.

**Resultado esperado:** la fotografía queda asociada a la visita.

**PASS:** la fotografía se almacena correctamente.

**FAIL:** se pierde o queda asociada incorrectamente.

---

### TEST-06

**Caso:** credenciales incorrectas.

**Resultado esperado:** acceso rechazado.

**PASS:** el sistema rechaza el acceso.

**FAIL:** el usuario obtiene acceso.

---

### TEST-07

**Caso:** API no disponible.

**Resultado esperado:** la aplicación gestiona el error sin bloquearse.

**PASS:** muestra un estado controlado y permite continuar cuando sea posible.

**FAIL:** la aplicación se bloquea o pierde datos.

---

## CRITERIOS DE ACEPTACIÓN

El fixture se considera válido cuando:

- el tipo APP-MOVIL se identifica correctamente;
- se reconocen los requisitos funcionales;
- se identifica la necesidad de backend;
- se identifica la API;
- se identifica el almacenamiento local;
- se identifica la sincronización;
- se contemplan seguridad y privacidad;
- se contemplan permisos;
- se contemplan notificaciones;
- existen pruebas verificables;
- existen pruebas negativas;
- la arquitectura no depende de una tecnología concreta sin justificación.

---

## PRUEBAS NEGATIVAS

El sistema debe detectar como problemas:

1. almacenar secretos del backend dentro de la aplicación;
2. permitir acceso con credenciales incorrectas;
3. perder datos registrados durante una desconexión;
4. duplicar registros durante la sincronización;
5. solicitar permisos que no correspondan a funciones reales;
6. transmitir información sensible sin protección;
7. permitir acceso no autorizado a visitas de otros usuarios.

---

## RESULTADO ESPERADO

```text
TIPO DETECTADO:
APP-MOVIL

RESULTADO:
PASS

COMPONENTES DETECTADOS:
- Aplicación móvil
- Backend
- API
- Base de datos
- Autenticación
- Almacenamiento local
- Sincronización
- Notificaciones
- Almacenamiento de imágenes
- Seguridad
- Privacidad

RIESGOS DETECTADOS:
- Sincronización
- Seguridad
- Privacidad
- Dependencia de servicios externos

PRUEBAS:
PASS
```

---

## ESTADO

**Estado:** Fixture inicial

**Versión:** 1.0


