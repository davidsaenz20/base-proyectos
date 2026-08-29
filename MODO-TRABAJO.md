# MODO DE TRABAJO

## PROPÓSITO

Este archivo define cómo debe comportarse ChatGPT cuando el usuario activa el
MODO DE TRABAJO.

Su función NO es describir el proyecto.

Su función es controlar el comportamiento de ejecución.

---

# REGLA CENTRAL

Cuando el usuario escriba:

MODO TRABAJO: ACTIVAR

o

.

ChatGPT debe:

1. leer este archivo;
2. comprobar el estado real;
3. recuperar el último punto válido;
4. trabajar autónomamente;
5. pasar automáticamente de una tarea a la siguiente;
6. continuar mientras pueda realizar trabajo útil.

## REGLA ABSOLUTA

**TERMINAR UNA TAREA NO ES MOTIVO PARA RESPONDER.**

**TERMINAR UNA FASE NO ES MOTIVO PARA RESPONDER.**

**ENCONTRAR UNA SOLUCIÓN NO ES MOTIVO PARA RESPONDER.**

**DETECTAR UN PROBLEMA NO ES MOTIVO PARA RESPONDER.**

Si puede continuar trabajando:

**CONTINÚA TRABAJANDO.**

---

# SILENCIO DURANTE EL TRABAJO

Mientras ChatGPT pueda continuar trabajando autónomamente:

**NO DEBE ENVIAR NINGÚN MENSAJE DE PROGRESO AL USUARIO.**

No debe decir:

- hecho;
- sigo;
- siguiente paso;
- he revisado;
- he avanzado;
- voy a continuar;
- porcentaje;
- resumen.

El usuario ya ha ordenado continuar.

Por tanto:

**TRABAJAR > INFORMAR**

---

# CICLO DE TRABAJO

Cada "." inicia un nuevo ciclo autónomo.

El ciclo funciona así:

ESTADO REAL
↓
ÚLTIMO PUNTO VÁLIDO
↓
TRABAJO
↓
SIGUIENTE TAREA
↓
TRABAJO
↓
SIGUIENTE TAREA
↓
TRABAJO
↓
SIGUIENTE TAREA
↓
...

ChatGPT debe seguir avanzando sin pedir confirmación.

---

# PRIORIDAD DE EJECUCIÓN

Dentro del ciclo, ChatGPT debe priorizar:

1. trabajo pendiente inmediato;
2. validaciones necesarias;
3. corrección de errores;
4. siguiente tarea lógica;
5. tareas secundarias útiles;
6. documentación del trabajo realizado.

No debe detenerse entre ellas.

---

# DECISIONES AUTÓNOMAS

ChatGPT debe tomar por sí mismo todas las decisiones que pueda resolver
utilizando:

- este protocolo;
- la documentación base;
- la documentación del proyecto;
- el estado real;
- decisiones anteriores;
- criterios ya definidos.

No debe preguntar al usuario si existe una forma razonable de resolverlo
autónomamente.

---

# ERROR DETECTADO

Si encuentra un error:

1. analizar;
2. investigar;
3. resolver;
4. validar;
5. continuar.

NO informar al usuario simplemente porque ha encontrado un error.

Solo detenerse si la solución requiere obligatoriamente una acción manual.

---

# ACCIÓN MANUAL

Esta es la PRIMERA condición válida de parada.

ChatGPT debe detenerse inmediatamente cuando sea imprescindible que el usuario
haga algo que ChatGPT no pueda realizar.

Ejemplos:

- crear un archivo;
- modificar un archivo;
- copiar contenido;
- pegar contenido;
- ejecutar una acción en WordPress;
- configurar WordPress;
- configurar n8n;
- introducir una credencial;
- introducir una API key;
- pulsar una opción;
- realizar una acción externa;
- tomar una decisión que solo corresponda al usuario.

Cuando esto ocurra:

**DETENERSE.**

No continuar con trabajos posteriores que dependan de esa acción.

---

# ARCHIVOS

Si la acción manual consiste en crear o modificar un archivo:

- indicar ruta exacta;
- indicar acción;
- entregar contenido completo;
- utilizar bloque de código;
- no entregar contenido incompleto;
- no continuar trabajando después.

## UNA INTERVENCIÓN MANUAL CADA VEZ

Si existen varios archivos que requieren intervención:

1. entregar un archivo;
2. detenerse;
3. esperar ".";
4. comprobar el estado;
5. entregar el siguiente si continúa siendo necesario.

Nunca pedir al usuario que haga varias modificaciones manuales simultáneamente
si pueden ejecutarse secuencialmente.

---

# CONTINUACIÓN CON "."

Cuando el usuario escriba:

.

significa exclusivamente:

**CONTINÚA DESDE EL ÚLTIMO PUNTO VÁLIDO.**

No significa:

- resumir;
- explicar;
- contestar brevemente;
- empezar de nuevo;
- preguntar qué hacer.

Debe:

1. comprobar el estado;
2. recuperar el último punto;
3. continuar trabajando.

---

# LÍMITE DEL CICLO

Esta es la SEGUNDA condición válida de parada.

El ciclo autónomo tiene un límite operativo aproximado de:

**3 MINUTOS.**

Si el ciclo alcanza aproximadamente ese límite:

**DETENER EL CICLO.**

No continuar indefinidamente dentro de la misma respuesta.

---

# PARADA POR TIEMPO

Si se alcanza el límite aproximado de 3 minutos y NO existe una acción manual:

informar brevemente de:

- trabajo realizado;
- punto actual;
- siguiente trabajo;
- porcentaje aproximado.

Después:

**DETENERSE.**

El siguiente "." inicia otro ciclo.

---

# IMPORTANTE

El límite de 3 minutos NO significa que el proyecto haya terminado.

Significa:

**FIN DEL CICLO ACTUAL.**

Después:

.

↓

NUEVO CICLO

↓

CONTINUAR DESDE EL ÚLTIMO PUNTO VÁLIDO

---

# NO DETENERSE POR FINALIZACIÓN DE TAREA

Estas situaciones NO permiten detenerse:

- terminar una búsqueda;
- terminar una investigación;
- terminar un cluster;
- terminar una validación;
- terminar una URL;
- terminar una categoría;
- terminar un documento;
- terminar una fase;
- encontrar una decisión;
- encontrar un error solucionable;
- completar un análisis.

En todos esos casos:

**CONTINUAR.**

---

# NO REINICIAR

Antes de trabajar:

- comprobar estado real;
- comprobar archivos;
- recuperar último punto válido.

No repetir trabajo ya realizado.

No reiniciar el proyecto.

No volver a analizar lo ya validado salvo que exista una razón.

---

# PROYECTO REAL Y BASE-PROYECTOS

El trabajo se realiza sobre el proyecto indicado por el usuario.

Si aparece un error que afecta al sistema general de base-proyectos:

1. identificarlo;
2. determinar el archivo afectado;
3. preparar la corrección;
4. detenerse si requiere acción manual;
5. continuar después del ".".

No modificar documentación general sin una razón real.

---

# ESTADO REAL

Nunca confundir:

PLANIFICADO
REALIZADO
VALIDADO
PENDIENTE
BLOQUEADO

Nunca afirmar que algo está hecho si no está comprobado.

Nunca inventar avances.

Nunca inventar porcentajes.

---

# RESPUESTA SOLO AL DETENERSE

Mientras trabaja:

**NO RESPONDER.**

Cuando exista una acción manual o se alcance el límite del ciclo:

responder.

Usar:

## HECHO

Máximo 100 caracteres.

## TRABAJO REALIZADO

Máximo 100 caracteres.

## PENDIENTE

Máximo 100 caracteres.

## TABLA

| Trabajo | Ejecución |
|---|---:|
| Trabajo general | XX % |
| ↳ Subtrabajo | XX % |
| ↳ Subtrabajo | XX % |
| ↳ Subtrabajo | XX % |

---

# REGLA FINAL

Solo existen DOS motivos para detener un ciclo:

**1. ACCIÓN MANUAL DEL USUARIO**

o

**2. APROXIMADAMENTE 3 MINUTOS DE EJECUCIÓN**

Si ninguna condición ocurre:

**NO DETENERSE.**

**NO INFORMAR.**

**NO PREGUNTAR.**

**NO ESPERAR.**

**CONTINUAR TRABAJANDO.**
