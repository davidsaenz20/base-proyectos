# FIXTURE — PRUEBA PROYECTO WEB DE AFILIACIÓN

## Identificación

**Nombre:** Proyecto Web de Afiliación Ejemplo

**Tipo:** WEB DE AFILIACIÓN

**Versión:** 1.0

**Estado de prueba:** NOT RUN

---

## 1. OBJETIVO

Comprobar que BASE-PROYECTOS puede analizar correctamente un proyecto web orientado a afiliación, identificar su naturaleza específica frente a una WEB convencional, seleccionar los módulos necesarios y producir una especificación coherente antes de construir.

Este fixture es ficticio y no representa un proyecto real.

---

## 2. ENTRADA

Crear una web especializada en recomendar productos de una categoría determinada mediante contenido informativo y enlaces de afiliación.

La web debe incluir:

- página principal;
- categorías;
- páginas de contenidos;
- fichas o páginas de recomendación;
- enlaces de afiliación;
- llamadas a la acción;
- información legal;
- versión móvil.

El sistema de afiliación debe poder identificarse como parte específica del proyecto.

---

## 3. CONTEXTO

**Usuario:** persona que busca información y recomendaciones antes de tomar una decisión de compra.

**Objetivo de negocio:** atraer usuarios mediante contenido útil y obtener ingresos mediante programas de afiliación.

**Tipo esperado:** WEB DE AFILIACIÓN.

**Complejidad:** media.

No se requiere necesariamente ecommerce propio, gestión de pedidos propios ni aplicación móvil.

La existencia de enlaces de afiliación no implica que el proyecto sea un ecommerce.

---

## 4. MÓDULOS PREVISTOS

Módulos potencialmente aplicables:

- Web;
- Contenido;
- SEO;
- Afiliación;
- Analítica;
- Email;
- Seguridad;
- Observabilidad.

El sistema debe comprobar cuáles son realmente necesarios.

No debe añadir módulos únicamente porque aparezcan en este fixture.

---

## 5. PROCESO ESPERADO

1. Identificar la entrada como un proyecto WEB DE AFILIACIÓN.
2. Diferenciarlo de una WEB convencional.
3. Extraer los requisitos funcionales.
4. Identificar el modelo de monetización por afiliación.
5. Determinar los módulos necesarios.
6. Identificar dependencias externas.
7. Definir una arquitectura proporcional a la complejidad.
8. Identificar requisitos legales y de seguridad relevantes.
9. Definir criterios de validación.
10. Identificar riesgos.
11. Producir una especificación previa a la construcción.

---

## 6. RESULTADO ESPERADO

El análisis debe producir como mínimo:

- tipo de proyecto identificado como WEB DE AFILIACIÓN;
- objetivo definido;
- usuario definido;
- requisitos funcionales;
- modelo de monetización identificado;
- módulos justificados;
- arquitectura propuesta;
- dependencias identificadas;
- criterios de validación;
- riesgos relevantes.

La arquitectura debe ser proporcional al proyecto.

No debe introducirse infraestructura innecesariamente compleja.

---

## 7. CRITERIOS PASS

La prueba será PASS si:

- identifica correctamente el tipo WEB DE AFILIACIÓN;
- no lo clasifica automáticamente como WEB convencional;
- no lo confunde con Ecommerce;
- identifica la finalidad de afiliación;
- identifica el modelo de monetización;
- identifica las funcionalidades solicitadas;
- selecciona únicamente módulos justificados;
- identifica las dependencias relevantes;
- contempla los requisitos legales pertinentes;
- propone una arquitectura coherente;
- define criterios de validación;
- identifica riesgos relevantes;
- no inventa información crítica;
- produce un resultado utilizable para iniciar diseño y construcción.

---

## 8. CRITERIOS FAIL

La prueba será FAIL si:

- clasifica incorrectamente el proyecto;
- ignora la finalidad de afiliación;
- confunde afiliación con ecommerce propio;
- omite funcionalidades obligatorias;
- añade módulos innecesarios como obligatorios;
- ignora dependencias externas relevantes;
- no contempla requisitos legales relevantes;
- no define criterios de validación;
- inventa información crítica;
- propone una arquitectura desproporcionada;
- considera terminada la validación sin comprobar los criterios definidos.

---

## 9. PRUEBAS NEGATIVAS

### Caso A — Ecommerce propio

Si la entrada añade carrito propio, pagos propios, gestión de pedidos y gestión de clientes, el sistema debe evaluar si el proyecto ha pasado a ser principalmente Ecommerce.

### Caso B — Web informativa sin afiliación

Si se elimina completamente la monetización mediante afiliación y el proyecto únicamente presenta información corporativa, el sistema debe evaluar si corresponde a WEB.

### Caso C — Aplicación móvil

Si la entrada exige instalación en dispositivos y funcionalidades nativas, el sistema debe evaluar APP MÓVIL.

### Caso D — Falta de información

Si no se conoce el objetivo, usuario, modelo de monetización o funcionalidad principal, el sistema no debe inventarlos.

Debe solicitar información o marcar la situación como REQUIERE VALIDACIÓN.

---

## 10. DEPENDENCIAS

Posibles dependencias:

- programas de afiliación;
- proveedores externos;
- enlaces de seguimiento;
- dominio;
- hosting;
- sistema de contenidos;
- analítica;
- herramientas SEO;
- email.

No todas son obligatorias.

Deben confirmarse durante el diseño.

---

## 11. RIESGOS

- enlaces de afiliación incorrectos;
- cambios en programas de afiliación;
- pérdida de atribución;
- contenido de baja calidad;
- contenido duplicado;
- dependencia de terceros;
- información incorrecta;
- problemas legales;
- mala experiencia de usuario;
- mala visualización móvil;
- rendimiento insuficiente;
- configuración de seguridad deficiente.

---

## 12. VALIDACIÓN FUNCIONAL

Comprobar:

1. La página principal carga correctamente.
2. Las categorías funcionan.
3. Las páginas de contenido son accesibles.
4. Las páginas de recomendación son accesibles.
5. Los enlaces de afiliación funcionan.
6. Los enlaces externos apuntan al destino esperado.
7. Las llamadas a la acción funcionan.
8. La web se visualiza correctamente en móvil.
9. La información legal está disponible.
10. No existen errores críticos visibles.

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

**Versión:** 1.0


