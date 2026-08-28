# PROTOCOLO DE EJECUCIÓN

## Objetivo

Definir el proceso para ejecutar un proyecto desde la idea inicial hasta su validación y puesta en funcionamiento.

## Fases

1. Analizar la idea.
2. Evaluar viabilidad.
3. Definir requisitos.
4. Diseñar la arquitectura.
5. Seleccionar módulos y plantillas.
6. Planificar la implementación.
7. Construir.
8. Probar.
9. Corregir.
10. Validar.
11. Desplegar.
12. Monitorizar.
13. Mejorar.

## Principio de ejecución

Cada fase debe producir un resultado verificable antes de considerar que la fase está completada.

El proceso debe avanzar de forma iterativa cuando una prueba detecte errores o nuevas necesidades.

## Control del proyecto

El estado del proyecto debe mantenerse sincronizado con:

- `00-CONTROL/ESTADO.md`
- `00-CONTROL/ROADMAP.md`
- `00-CONTROL/DECISIONES.md`
- `00-CONTROL/INVENTARIO-DOCUMENTOS.md`

## Uso de plantillas

Las plantillas de `03-PLANTILLAS/` deben reutilizarse cuando sean aplicables.

No se debe crear una estructura nueva si una plantilla existente puede resolver la necesidad sin introducir complejidad innecesaria.

## Uso de módulos

Los módulos de `02-MODULOS/` deben utilizarse cuando aporten una capacidad necesaria para el proyecto.

Los módulos deben mantenerse independientes y reutilizables siempre que sea posible.

## Tipo de proyecto

Antes de iniciar la construcción debe identificarse el tipo de proyecto y consultar el documento correspondiente dentro de `04-TIPOS-PROYECTO/`.

## Fixtures

Cuando exista un fixture aplicable en `05-FIXTURES/`, debe utilizarse para validar que la metodología puede ejecutarse correctamente.

## Validación

La finalización de una fase no debe basarse únicamente en que exista documentación.

Debe existir evidencia suficiente de que el resultado funciona según los requisitos definidos.

## Corrección de errores

Cuando una prueba detecte un error:

1. registrar el problema;
2. identificar la causa;
3. determinar la corrección;
4. aplicar la corrección;
5. repetir la validación.

## Referencias documentales

Las rutas utilizadas en este documento deben corresponder siempre a la estructura real del repositorio.

La documentación de control se encuentra en `00-CONTROL/`.

El roadmap oficial es:

`00-CONTROL/ROADMAP.md`

## Criterio de finalización

Un proyecto solo puede considerarse finalizado cuando:

- los requisitos principales están cubiertos;
- las pruebas necesarias se han ejecutado;
- los errores críticos están resueltos;
- el despliegue previsto se ha realizado cuando corresponda;
- el resultado ha sido validado;
- la documentación necesaria está actualizada.

- 
