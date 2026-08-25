

# PLANTILLA DE ARQUITECTURA

> Documento que define cómo estará construido el proyecto antes y durante su implementación.
>
> No controla el estado operativo del proyecto.
>
> El estado actual se registra exclusivamente en:
>
> `00-CONTROL/ESTADO.md`

---

# 1. OBJETIVO

**Objetivo de la arquitectura:**

**Problemas técnicos que debe resolver:**

---

# 2. VISIÓN GENERAL

**Descripción de la solución:**

**Principios arquitectónicos:**

- 

---

# 3. COMPONENTES

## Componente 001

**Nombre:**

**Función:**

**Tecnología:**

**Dependencias:**

**Entrada:**

**Salida:**

---

## Componente 002

**Nombre:**

**Función:**

**Tecnología:**

**Dependencias:**

**Entrada:**

**Salida:**

---

# 4. FLUJO DEL SISTEMA

Describir cómo circulan los datos y las acciones entre los componentes.

```text
ENTRADA
   ↓
PROCESAMIENTO
   ↓
ALMACENAMIENTO / INTEGRACIÓN
   ↓
SALIDA

Flujo detallado:

1. 
2. 
3. 


---

5. DATOS

Datos de entrada:

Datos procesados:

Datos de salida:

Almacenamiento:

Retención:

Eliminación:


---

6. INTEGRACIONES

Servicio	Función	Entrada	Salida	Dependencia

				



---

7. APIS

API	Función	Método	Entrada	Salida

				



---

8. SEGURIDAD

Autenticación:

Autorización:

Credenciales y secretos:

Protección de datos:

Transporte seguro:

Riesgos relevantes:


---

9. ERRORES Y RECUPERACIÓN

Errores previsibles:


Comportamiento ante error:


Reintentos:

Fallback:

Recuperación:


---

10. ESCALABILIDAD

Necesidades previstas:

Limitaciones conocidas:

Puntos de escalabilidad:


---

11. DISPONIBILIDAD

Nivel esperado:

Dependencias críticas:

Puntos únicos de fallo:

Recuperación ante caída:


---

12. COSTES

Infraestructura:

Servicios externos:

APIs:

Mantenimiento:

Coste estimado total:


---

13. DECISIONES TÉCNICAS

DEC-001

Decisión:

Motivo:

Alternativas consideradas:

Consecuencia:


---

14. RIESGOS ARQUITECTÓNICOS

RISK-001

Riesgo:

Probabilidad:

Impacto:

Mitigación:


---

15. DEPENDENCIAS EXTERNAS


Para cada dependencia crítica:

Servicio:

Función:

Proveedor:

Alternativa:

Impacto si deja de funcionar:


---

16. VALIDACIÓN DE LA ARQUITECTURA

La arquitectura debe validarse antes de considerarse lista para construcción.

Comprobaciones

[ ] Todos los requisitos críticos tienen una solución arquitectónica.

[ ] Los componentes principales están definidos.

[ ] Las integraciones están identificadas.

[ ] Los datos están definidos.

[ ] La seguridad está contemplada.

[ ] Los errores y la recuperación están contemplados.

[ ] Las dependencias externas están identificadas.

[ ] Los costes relevantes han sido considerados.

[ ] El despliegue previsto es técnicamente viable.

[ ] El flujo completo puede ejecutarse de extremo a extremo.


Resultado

Resultado de la validación:

Pendiente

Parcial

Validada

Validada con incidencias aceptadas


Evidencias:



---

17. CRITERIOS DE ACEPTACIÓN

La arquitectura se considera preparada para construcción cuando:



---

18. VERSIONADO

Versión de arquitectura:

Fecha:

Motivo del cambio:


---

19. NOTAS



---

REGLA

Esta plantilla responde a:

¿CÓMO ESTÁ CONSTRUIDO EL SISTEMA?

¿CÓMO CIRCULAN LOS DATOS?

¿CÓMO SE INTEGRAN LOS COMPONENTES?

¿CÓMO SE PROTEGE?

¿CÓMO SE RECUPERA DE LOS ERRORES?

¿CÓMO SABEMOS QUE LA ARQUITECTURA ES VIABLE?

No responde a:

¿EN QUÉ FASE ESTÁ EL PROYECTO?

Esa información pertenece exclusivamente a:

00-CONTROL/ESTADO.md
