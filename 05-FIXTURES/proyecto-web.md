# FIXTURE — PRUEBA PROYECTO WEB

## Identificación

**Nombre:** Proyecto Web Ejemplo

**Tipo:** WEB

**Versión:** 2.0

**Estado de prueba:** NOT RUN

---

## 1. OBJETIVO

Comprobar que BASE-PROYECTOS puede analizar una solicitud de una web empresarial sencilla, identificar correctamente el tipo de proyecto, seleccionar módulos razonables y producir una especificación coherente antes de construir.

Este fixture es ficticio y no representa un proyecto real.

---

## 2. ENTRADA

Crear una web para una empresa ficticia que necesita presentar sus servicios y recibir solicitudes de contacto.

La web debe incluir:

- página principal;
- página de servicios;
- página de contacto;
- formulario de contacto;
- información de contacto;
- versión móvil.

---

## 3. CONTEXTO

**Usuario:** persona que busca información sobre los servicios de la empresa.

**Objetivo de negocio:** presentar los servicios y facilitar el contacto.

**Tipo esperado:** WEB.

**Complejidad:** baja.

No se requiere ecommerce, área privada, aplicación móvil ni funcionalidades avanzadas.

---

## 4. MÓDULOS PREVISTOS

Módulos potencialmente aplicables:

- Web;
- Email;
- Seguridad;
- Observabilidad.

El sistema debe comprobar si todos son realmente necesarios antes de seleccionarlos.

No debe añadir módulos únicamente por aparecer en este fixture.

---

## 5. PROCESO ESPERADO

1. Identificar la entrada como un proyecto de tipo WEB.
2. Extraer los requisitos funcionales.
3. Separar requisitos obligatorios de elementos opcionales.
4. Determinar los módulos necesarios.
5. Definir una arquitectura proporcional a la complejidad.
6. Identificar requisitos básicos de seguridad.
7. Definir las validaciones necesarias.
8. Identificar posibles dependencias o riesgos.
9. Producir una especificación previa a la construcción.

---

## 6. RESULTADO ESPERADO

El análisis debe producir como mínimo:

- tipo de proyecto identificado como WEB;
- objetivo definido;
- usuario definido;
- requisitos funcionales identificados;
- módulos justificados;
- arquitectura propuesta;
- criterios de validación;
- riesgos o dependencias relevantes.

La arquitectura debe ser proporcional al proyecto.

No debe introducirse una infraestructura innecesariamente compleja.

---

## 7. CRITERIOS PASS

La prueba será PASS si se cumplen todos los criterios obligatorios:

- identifica correctamente el tipo WEB;
- no confunde el proyecto con SaaS, Ecommerce o App Móvil;
- identifica las funcionalidades solicitadas;
- distingue requisitos obligatorios de opcionales;
- selecciona únicamente módulos justificados;
- propone una arquitectura coherente con una web sencilla;
- incluye validación de navegación;
- incluye validación del formulario;
- incluye validación móvil;
- incluye comprobación de enlaces;
- contempla seguridad básica;
- identifica dependencias relevantes cuando existan;
- no inventa requisitos no proporcionados;
- produce un resultado utilizable para iniciar la fase de diseño/construcción.

---

## 8. CRITERIOS FAIL

La prueba será FAIL si ocurre cualquiera de los siguientes casos:

- clasifica el proyecto como otro tipo;
- ignora una funcionalidad obligatoria;
- añade complejidad sin justificación;
- selecciona módulos incompatibles o innecesarios como obligatorios;
- no define criterios de validación;
- inventa información crítica;
- omite requisitos básicos de seguridad;
- considera terminada la validación sin comprobar los criterios definidos.

---

## 9. PRUEBAS NEGATIVAS

El sistema debe poder detectar correctamente estos escenarios:

### Caso A — Ecommerce oculto

Si la entrada añade pagos, carrito y gestión de pedidos, el sistema debe detectar que el alcance ya no corresponde a una web empresarial sencilla y evaluar el tipo Ecommerce.

### Caso B — Área privada compleja

Si la entrada añade cuentas, roles, datos aislados por cliente y facturación recurrente, el sistema debe evaluar si corresponde a SaaS.

### Caso C — Aplicación móvil

Si la entrada exige instalación en dispositivos y funcionalidades nativas, el sistema debe evaluar el tipo APP MÓVIL.

### Caso D — Falta de información

Si no se conoce el objetivo, usuario ni funcionalidad principal, el sistema no debe inventarlos. Debe solicitar información o marcar la situación como REQUIERE VALIDACIÓN.

---

## 10. DEPENDENCIAS

Posibles dependencias:

- proveedor de email;
- hosting;
- dominio;
- sistema de formularios;
- herramientas de analítica si se requieren.

No todas son obligatorias.

Deben confirmarse durante el diseño.

---

## 11. RIESGOS

- formulario mal configurado;
- mensajes no entregados;
- enlaces rotos;
- mala visualización móvil;
- rendimiento insuficiente;
- configuración de seguridad deficiente;
- publicación de información incorrecta.

---

## 12. VALIDACIÓN FUNCIONAL

Comprobar:

1. La página principal carga correctamente.
2. La navegación entre páginas funciona.
3. La página de servicios es accesible.
4. El formulario puede completarse.
5. El formulario produce el resultado esperado.
6. La información de contacto es visible.
7. Los enlaces funcionan.
8. La web se visualiza correctamente en móvil.
9. No existen errores críticos visibles.

---

## 13. RESULTADO DE LA PRUEBA

**Estado:** NOT RUN

**Fecha:** Pendiente.

**Resultado observado:** Pendiente.

**Incidencias:** Pendiente.

**Correcciones necesarias:** Pendiente.

---

## 14. REGLA DEL FIXTURE

Este fixture no demuestra por sí mismo que BASE-PROYECTOS funcione.

Solo se considerará validado cuando se ejecute la prueba y se comprueben sus criterios PASS/FAIL.

---

## ESTADO

**Estado:** Fixture verificable

**Versión:** 2.0
