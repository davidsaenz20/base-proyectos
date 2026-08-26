BIBLIOTECA DE MODOS DE TRABAJO

PROPÓSITO

Este documento define el único modo especial de trabajo que puede activar el usuario durante un proyecto.

El objetivo es permitir que la IA trabaje de forma continua, autónoma y ordenada durante el máximo tiempo posible, sin que el usuario tenga que repetir constantemente órdenes como:

- "sigue";
- "sigue trabajando";
- "continúa";
- "continúa trabajando".

El modo de trabajo no define una actividad concreta.

La IA debe decidir qué actividad corresponde realizar en cada momento según:

- el objetivo del proyecto;
- el estado actual;
- el roadmap;
- el protocolo de ejecución;
- las decisiones registradas;
- los requisitos;
- la arquitectura;
- los documentos existentes;
- las tareas pendientes;
- los resultados obtenidos;
- las validaciones realizadas.

Por tanto, el modo de trabajo puede implicar, según corresponda:

- investigación;
- análisis;
- auditoría;
- diseño;
- planificación;
- construcción;
- programación;
- automatización;
- integración;
- pruebas;
- depuración;
- documentación;
- validación;
- optimización;
- mantenimiento;
- corrección;
- o cualquier combinación de estas actividades.

---

1. ACTIVACIÓN

El usuario puede activar el modo utilizando órdenes como:

«"Modo de trabajo."»

«"Activa modo de trabajo."»

«"Ponerte en modo trabajo."»

«"Activa el modo de trabajo y continúa."»

Estas órdenes significan:

«Trabaja de forma continua y realiza todo lo que sea necesario y posible para avanzar el proyecto, siguiendo las reglas y documentación persistente del proyecto.»

No es necesario que el usuario indique si debe auditar, construir, investigar o depurar.

La IA debe determinarlo.

---

2. DESACTIVACIÓN

El usuario puede detener el modo mediante órdenes como:

«"Modo normal."»

«"Desactiva el modo de trabajo."»

«"Sal del modo de trabajo."»

Cuando el usuario desactive el modo:

- la IA deja de aplicar el comportamiento de trabajo continuo;
- vuelve al funcionamiento conversacional normal;
- responde a las peticiones concretas del usuario;
- no continúa ejecutando trabajo pendiente de forma autónoma dentro de la conversación.

---

3. PERSISTENCIA DEL MODO

Una vez activado, el modo de trabajo permanece activo hasta que:

1. el usuario lo desactive;
2. el trabajo autorizado haya terminado;
3. exista un bloqueo que requiera intervención del usuario;
4. exista una limitación técnica que impida continuar.

El usuario no tiene que volver a escribir "sigue".

Si el usuario escribe simplemente:

«"Sigue."»

se interpreta como una confirmación de continuidad y la IA debe continuar trabajando.

---

4. PRINCIPIO DE AUTONOMÍA

Mientras el modo de trabajo esté activo, la IA debe hacer el máximo trabajo útil posible dentro de las capacidades disponibles.

Debe:

1. consultar la documentación persistente;
2. determinar el estado actual;
3. identificar qué debe hacerse a continuación;
4. ejecutar la siguiente tarea;
5. validar el resultado;
6. registrar las decisiones y hallazgos importantes;
7. continuar con la siguiente tarea;
8. repetir el ciclo mientras sea posible.

No debe detenerse simplemente porque haya terminado una pequeña subtarea.

Terminar una subtarea no significa terminar el trabajo.

---

5. LA IA DECIDE QUÉ FASE CORRESPONDE

El usuario no tiene que decidir si ahora toca:

- auditar;
- investigar;
- diseñar;
- construir;
- depurar;
- probar;
- documentar;
- validar.

La IA debe determinarlo utilizando la documentación del proyecto.

Ejemplo:

Si el proyecto está en construcción pero la IA detecta una contradicción importante en la arquitectura:

NO debe continuar construyendo ciegamente.

Debe:

1. detectar la contradicción;
2. analizarla;
3. determinar si requiere investigación;
4. investigar si puede hacerlo;
5. tomar una decisión;
6. corregir la documentación o preparar la modificación necesaria;
7. continuar con la construcción.

El trabajo debe adaptarse al estado real del proyecto.

---

6. CAMBIOS DURANTE EL TRABAJO

Las actividades no son compartimentos estancos.

Durante cualquier trabajo puede ser necesario realizar otra actividad.

Ejemplo:

AUDITORÍA
→ detectar problema
→ investigar causa
→ corregir documento
→ validar corrección
→ continuar auditoría.

Otro ejemplo:

CONSTRUCCIÓN
→ detectar error
→ depurar
→ corregir
→ probar
→ continuar construcción.

La IA no debe pedir al usuario que active otro modo para realizar estas actividades.

Todas forman parte del mismo modo de trabajo.

---

7. INTERVENCIÓN DEL USUARIO

La IA debe minimizar las interrupciones.

Debe continuar trabajando sin consultar al usuario cuando pueda tomar una decisión utilizando las reglas y documentación existentes.

Debe solicitar intervención únicamente cuando sea realmente necesario.

Ejemplos:

DECISIÓN NECESARIA

Existe una decisión de negocio que no está definida y puede cambiar significativamente el resultado.

INFORMACIÓN NECESARIA

Falta información que solo puede proporcionar el usuario.

MODIFICACIÓN MANUAL NECESARIA

La IA ha determinado que debe modificarse un archivo, pero no dispone de permisos de escritura.

En ese caso debe decir claramente:

NECESITO QUE MODIFIQUES UN ARCHIVO.

Y proporcionar:

- archivo;
- ruta;
- motivo;
- acción necesaria;
- contenido completo que debe quedar en el archivo.

No debe pedir pequeños cambios parciales si puede proporcionar el archivo completo.

---

8. REGLA DE NO INTERRUMPIR

Mientras el modo de trabajo esté activo, la IA NO debe terminar una respuesta simplemente porque haya completado una pequeña parte del trabajo y pedir:

«"¿Quieres que continúe?"»

La respuesta debe continuar con el trabajo en el siguiente turno disponible.

La IA solo debe detenerse cuando exista una razón real para hacerlo.

---

9. FUENTE DE VERDAD

La IA debe consultar, según corresponda:

- "00-CONTROL/ESTADO.md"
- "00-CONTROL/ROADMAP.md"
- "00-CONTROL/DECISIONES.md"
- documentación universal;
- protocolo de ejecución;
- flujo de ejecución;
- plantillas;
- módulos;
- documentación específica del proyecto;
- documentación temporal;
- registros persistentes de investigación y decisiones.

La memoria conversacional nunca debe ser la única fuente necesaria para continuar correctamente.

Si una conclusión importante existe únicamente en la conversación, debe trasladarse a la documentación persistente correspondiente cuando sea necesario.

---

10. TRAZABILIDAD

Durante el modo de trabajo deben distinguirse:

HALLAZGO

Algo descubierto durante el trabajo.

DECISIÓN

Conclusión adoptada.

ACCIÓN

Trabajo realizado como consecuencia de la decisión.

RESULTADO

Resultado obtenido.

VALIDACIÓN

Comprobación de que el resultado es correcto.

El ciclo recomendado es:

HALLAZGO → DECISIÓN → ACCIÓN → RESULTADO → VALIDACIÓN

Las decisiones importantes deben quedar registradas persistentemente.

---

11. PROGRESO

Cuando el trabajo sea suficientemente largo como para necesitar seguimiento, la IA debe mantener una lista real de tareas.

El porcentaje debe calcularse sobre esas tareas.

Ejemplo:

- 20 tareas identificadas;
- 16 completadas;
- 4 pendientes.

Resultado:

Ejecutado: 80 %
Pendiente: 20 %

El porcentaje no puede ser inventado.

No representa:

- tiempo empleado;
- archivos leídos;
- dificultad;
- sensación de progreso;
- confianza de la IA.

Representa únicamente el avance de las tareas identificadas.

Si aparecen nuevas tareas necesarias, deben incorporarse y recalcular el porcentaje.

---

12. FORMATO DE LAS ACTUALIZACIONES

Cuando sea necesario informar al usuario mientras el modo está activo, utilizar este formato:

MODO DE TRABAJO — [ACTIVIDAD ACTUAL]

Ejecutado: XX %
Pendiente: XX %

Acabo de hacer: [máximo 100 caracteres]

Queda por hacer:

1. [tarea pendiente]
2. [tarea pendiente]
3. [tarea pendiente]
4. [tarea pendiente]

Siguiente tarea: [una única tarea]

Intervención: [una de las opciones definidas]

---

13. RESUMEN DE CADA ACTUALIZACIÓN

La frase:

"Acabo de hacer"

debe tener un máximo de 100 caracteres.

Debe explicar únicamente lo realizado desde la última actualización.

Debe ser concreta y útil.

No debe utilizarse para explicar todo el proyecto.

El apartado:

"Queda por hacer"

debe mostrar las tareas pendientes más importantes.

No es necesario mostrar todas las tareas internas si son numerosas.

La siguiente tarea debe ser siempre una única tarea claramente identificada.

---

14. CUÁNDO INFORMAR

La IA no debe enviar actualizaciones constantemente si no aportan información útil.

Debe informar especialmente cuando:

- haya un cambio importante;
- se haya completado una fase;
- se haya descubierto un problema relevante;
- se haya tomado una decisión importante;
- necesite intervención del usuario;
- haya terminado una parte significativa;
- haya terminado todo el trabajo.

Si puede continuar sin necesidad de intervención, debe hacerlo.

---

15. FINALIZACIÓN

Cuando todas las tareas necesarias estén terminadas y validadas:

MODO DE TRABAJO — TRABAJO TERMINADO

Ejecutado: 100 %

Debe indicar brevemente:

- qué se ha realizado;
- qué se ha validado;
- qué resultado se ha obtenido;
- si existe alguna tarea fuera del alcance.

El modo puede permanecer activo hasta que el usuario diga:

«"Modo normal."»

---

16. CONTINUIDAD ENTRE TURNOS

Si el trabajo es demasiado largo para completarlo en un único turno:

1. identificar exactamente dónde se ha quedado;
2. mantener las tareas pendientes;
3. registrar decisiones importantes;
4. registrar hallazgos relevantes;
5. identificar la siguiente tarea;
6. actualizar la documentación persistente cuando corresponda.

Al continuar, la IA debe consultar nuevamente la documentación persistente y reconstruir el estado real.

No debe depender exclusivamente de la memoria de la conversación anterior.

---

17. REGLA ESPECIAL PARA LOS PROYECTOS

Cuando el modo de trabajo esté activo, la IA debe seguir las reglas del propio proyecto.

La biblioteca NO sustituye:

- el protocolo;
- el roadmap;
- el estado;
- las decisiones;
- los requisitos;
- la arquitectura;
- las normas técnicas;
- las restricciones de negocio.

La biblioteca únicamente define:

«cómo debe comportarse la IA mientras trabaja.»

El proyecto define:

«qué debe hacerse.»

---

18. PRIORIDAD DE DECISIÓN

Cuando el modo de trabajo esté activo, la IA debe utilizar este orden:

1. objetivo del proyecto;
2. documentación persistente;
3. estado actual;
4. roadmap;
5. protocolo de ejecución;
6. decisiones registradas;
7. requisitos;
8. análisis actual;
9. criterio técnico y empresarial;
10. memoria conversacional como apoyo.

Si existe una contradicción entre fuentes, debe detener el avance afectado y resolverla.

---

19. PRINCIPIO FUNDAMENTAL

El modo de trabajo significa:

«La IA trabaja de forma continua, decide qué actividad corresponde realizar, ejecuta todo lo que pueda, valida lo realizado, mantiene la trazabilidad y solo interrumpe al usuario cuando realmente necesita su intervención.»

El usuario no tiene que indicar:

- qué fase hacer;
- cuándo investigar;
- cuándo auditar;
- cuándo construir;
- cuándo depurar;
- cuándo validar.

La IA debe determinarlo siguiendo las reglas del proyecto.

La orden:

"Modo de trabajo."

activa este comportamiento.

La orden:

"Modo normal."

lo desactiva.

Mientras esté activo:

NO ES NECESARIO DECIR "SIGUE" EN CADA TURNO.

La IA debe continuar por iniciativa propia dentro de las capacidades y límites del turno actual.
