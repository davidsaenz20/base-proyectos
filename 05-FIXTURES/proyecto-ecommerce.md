# FIXTURE PROYECTO ECOMMERCE

## Identificación

**Nombre:** Ecommerce de ejemplo

**Tipo:** Ecommerce

**Versión:** 2.0

**Estado de la prueba:** NOT RUN

---

## Objetivo

Comprobar que BASE-PROYECTOS puede analizar correctamente un proyecto de tipo Ecommerce, identificar sus necesidades, seleccionar los módulos adecuados, detectar dependencias y riesgos, y producir una estructura de proyecto coherente.

Este fixture es un entorno controlado de prueba.

No representa un ecommerce real.

---

## Entrada

Crear una tienda online ficticia que permita:

1. consultar productos;
2. buscar productos;
3. añadir productos al carrito;
4. completar un checkout;
5. realizar un pago;
6. recibir confirmación;
7. gestionar pedidos.

### Datos de entrada controlados

**Tipo de proyecto:** Ecommerce

**Usuarios:** clientes que desean consultar y comprar productos.

**Contenido principal:** productos, categorías, clientes, pedidos, pagos e inventario.

**Resultado solicitado:** definición estructurada del proyecto y de los elementos necesarios para su construcción y validación.

---

## Contexto

El proyecto debe proporcionar un canal de venta online para un catálogo ficticio.

Debe contemplar como mínimo:

- catálogo;
- productos;
- categorías;
- búsqueda;
- carrito;
- checkout;
- pagos;
- pedidos;
- usuarios;
- seguridad;
- mantenimiento;
- escalabilidad.

No se presupone una tecnología concreta.

La arquitectura debe determinarse a partir de los requisitos reales.

---

## Problema

El negocio necesita ofrecer sus productos mediante un canal de venta online.

El usuario debe poder completar el proceso desde la consulta del catálogo hasta la confirmación del pedido.

---

## Usuario

Cliente que desea consultar y comprar productos.

Puede existir un segundo tipo de usuario para la gestión del negocio.

Las funcionalidades específicas de administración deberán determinarse durante el análisis.

---

## Propuesta

Una tienda online organizada mediante:

- catálogo;
- categorías;
- búsqueda;
- carrito;
- checkout;
- pago;
- pedidos;
- gestión de usuarios.

La propuesta debe mantenerse dentro del alcance definido por la entrada.

No deben incorporarse funcionalidades no justificadas.

---

## Módulos

Módulos potencialmente implicados:

- Ecommerce
- Web
- Base de datos
- APIs
- Email
- Notificaciones
- Seguridad
- Observabilidad

La prueba debe comprobar que BASE-PROYECTOS:

1. identifica los módulos necesarios;
2. diferencia los necesarios de los opcionales;
3. identifica dependencias;
4. justifica su utilización;
5. evita incorporar módulos sin justificación.

---

## Datos

Una estructura de datos puede contener:

- productos;
- categorías;
- clientes;
- pedidos;
- líneas de pedido;
- pagos;
- inventario;
- estados;
- fechas.

Los campos definitivos deben determinarse durante el análisis.

No deben inventarse datos reales.

---

## Proceso esperado

### Paso 1. Identificación

Identificar el proyecto como:

**Tipo: Ecommerce**

### Paso 2. Análisis

Analizar:

- objetivo;
- usuarios;
- catálogo;
- productos;
- búsqueda;
- carrito;
- checkout;
- pago;
- pedidos;
- datos;
- seguridad;
- mantenimiento.

### Paso 3. Requisitos

Determinar los requisitos funcionales y no funcionales necesarios.

### Paso 4. Módulos

Seleccionar los módulos correspondientes y justificar su utilización.

### Paso 5. Dependencias

Identificar dependencias entre:

- catálogo;
- base de datos;
- web;
- carrito;
- checkout;
- pagos;
- APIs;
- email;
- seguridad;
- observabilidad.

### Paso 6. Arquitectura

Definir una arquitectura coherente con los requisitos.

No establecer una tecnología concreta sin justificación.

### Paso 7. Construcción

Definir los elementos necesarios para construir el proyecto.

### Paso 8. Validación

Definir las pruebas necesarias para comprobar:

- catálogo;
- búsqueda;
- carrito;
- checkout;
- pago;
- confirmación;
- pedidos;
- errores;
- comportamiento móvil.

### Paso 9. Resultado

Producir una definición estructurada del proyecto que permita continuar con las siguientes fases de BASE-PROYECTOS.

---

## Resultado esperado

La ejecución correcta debe producir como mínimo:

1. identificación del tipo Ecommerce;
2. objetivo definido;
3. usuarios identificados;
4. requisitos principales;
5. módulos necesarios;
6. dependencias;
7. riesgos;
8. arquitectura propuesta;
9. proceso de construcción;
10. validaciones;
11. criterios PASS/FAIL;
12. estado final de la prueba.

El resultado debe ser coherente con la información de entrada.

---

## Criterios PASS

La prueba será PASS si:

- identifica correctamente el tipo Ecommerce;
- mantiene el alcance;
- identifica las necesidades principales;
- selecciona módulos justificados;
- identifica dependencias relevantes;
- identifica riesgos relevantes;
- define una arquitectura coherente;
- define un proceso de construcción;
- define validaciones concretas;
- establece criterios PASS/FAIL;
- no inventa información no proporcionada;
- produce todos los elementos obligatorios del protocolo.

---

## Criterios FAIL

La prueba será FAIL si:

- identifica incorrectamente el tipo de proyecto;
- omite necesidades fundamentales;
- utiliza módulos sin justificación;
- ignora dependencias importantes;
- ignora riesgos relevantes;
- propone una arquitectura incompatible;
- omite la validación;
- utiliza criterios subjetivos sin condiciones comprobables;
- inventa información no proporcionada;
- no produce alguno de los elementos obligatorios;
- contradice reglas de BASE-PROYECTOS.

---

## Pruebas positivas

### PRUEBA POSITIVA 01 — Compra completa

**Entrada:**

Tienda online con catálogo, carrito, checkout y pago.

**Resultado esperado:**

Identificación correcta como Ecommerce y definición de un flujo completo de compra.

**PASS si:**

- identifica Ecommerce;
- identifica catálogo;
- identifica carrito;
- identifica checkout;
- identifica pago;
- identifica pedido;
- define validación.

**Estado:** NOT RUN

---

## Pruebas negativas

### PRUEBA NEGATIVA 01 — Información insuficiente

**Entrada:**

"Crear una tienda online."

**Resultado esperado:**

El sistema debe detectar que falta información suficiente para definir correctamente el proyecto.

Debe solicitar información adicional o marcar los elementos que requieren validación.

**PASS si:**

- no inventa requisitos;
- identifica la información que falta;
- marca el proyecto como pendiente de validación.

**Estado:** NOT RUN

---

### PRUEBA NEGATIVA 02 — Requisitos contradictorios

**Entrada:**

Crear una tienda en la que los usuarios puedan comprar productos, pero simultáneamente no puedan consultar ningún producto ni introducir datos del pedido.

**Resultado esperado:**

Detectar la contradicción y solicitar aclaración antes de definir una arquitectura definitiva.

**PASS si:**

- identifica la contradicción;
- no la ignora;
- no inventa una solución;
- solicita validación.

**Estado:** NOT RUN

---

## Pruebas de combinación

### COMBINACIÓN 01

Módulos:

- Ecommerce
- Web
- Base de datos
- API
- Email
- Notificaciones
- Seguridad
- Observabilidad

**Debe comprobarse:**

- responsabilidades;
- dependencias;
- flujo de datos;
- seguridad;
- coherencia arquitectónica.

**Estado:** NOT RUN

---

## Riesgos

Riesgos que deben evaluarse:

- datos duplicados;
- datos incorrectos;
- inventario desactualizado;
- errores de pago;
- pedidos duplicados;
- pérdida de pedidos;
- errores de checkout;
- crecimiento del catálogo;
- crecimiento del tráfico;
- problemas de seguridad;
- exposición de datos personales;
- disponibilidad de APIs externas;
- errores de notificación.

No todos los riesgos deben considerarse presentes.

Deben evaluarse según el proyecto real.

---

## Dependencias

Posibles dependencias:

- base de datos;
- sistema de pagos;
- API de pagos;
- sistema de email;
- sistema de notificaciones;
- catálogo;
- inventario;
- autenticación;
- web;
- monitorización.

Cada dependencia debe validarse antes de considerarla disponible.

---

## Seguridad

Debe evaluarse:

- protección de cuentas;
- protección de datos personales;
- gestión de credenciales;
- protección de información de pago;
- control de acceso;
- validación de entradas;
- protección de APIs;
- registros;
- prevención de abusos.

Las medidas definitivas deben determinarse durante el diseño.

---

## Escalabilidad

Debe evaluarse el comportamiento ante el crecimiento de:

- productos;
- categorías;
- clientes;
- pedidos;
- tráfico;
- consultas;
- volumen de datos.

La solución de escalabilidad debe definirse según las necesidades reales.

---

## Validación funcional

Debe comprobarse como mínimo:

### Catálogo

**Entrada:**

Acceso al catálogo.

**Resultado esperado:**

Los productos disponibles pueden consultarse.

### Búsqueda

**Entrada:**

Búsqueda de un producto.

**Resultado esperado:**

Se muestran resultados relevantes.

### Carrito

**Entrada:**

Añadir un producto al carrito.

**Resultado esperado:**

El producto aparece correctamente en el carrito.

### Checkout

**Entrada:**

Confirmar una compra.

**Resultado esperado:**

El proceso de checkout puede completarse correctamente.

### Pago

**Entrada:**

Realizar un pago de prueba.

**Resultado esperado:**

El resultado del pago se registra correctamente.

### Confirmación

**Entrada:**

Pago aprobado.

**Resultado esperado:**

El usuario recibe una confirmación y el pedido queda registrado.

### Pedidos

**Entrada:**

Consultar un pedido realizado.

**Resultado esperado:**

La información del pedido es coherente.

### Navegación móvil

**Entrada:**

Acceso mediante dispositivo móvil.

**Resultado esperado:**

Las funciones principales son utilizables.

---

## Resultado de la prueba

**Estado actual:** NOT RUN

La existencia de este fixture no significa que la prueba haya sido ejecutada.

Los resultados solo podrán cambiar a:

- PASS;
- FAIL;
- BLOCKED;

después de ejecutar y registrar las pruebas correspondientes.

---

## Registro de ejecución

**Fecha:** Pendiente

**Prueba ejecutada:** Pendiente

**Resultado:** NOT RUN

**Problemas detectados:** Pendiente

**Causa:** Pendiente

**Archivo o módulo afectado:** Pendiente

**Corrección propuesta:** Pendiente

**Nueva prueba necesaria:** Pendiente

---

## Repetibilidad

Las pruebas deben poder repetirse utilizando la misma entrada.

Cuando una prueba dependa de información externa cambiante, debe registrarse:

- fuente;
- fecha;
- versión;
- condición relevante.

---

## Estado

**Estado del fixture:** Verificable

**Estado de ejecución:** NOT RUN

**Versión:** 2.0

**Última revisión:** 2026-08-28

---

## Notas

Este archivo es un fixture controlado.

No representa un ecommerce real.

No demuestra por sí mismo que BASE-PROYECTOS funcione correctamente.

Su función es proporcionar un escenario reproducible para comprobar el comportamiento de BASE-PROYECTOS ante un proyecto de tipo Ecommerce.

