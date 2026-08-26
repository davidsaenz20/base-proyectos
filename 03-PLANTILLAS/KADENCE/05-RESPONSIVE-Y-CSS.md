

# KADENCE — RESPONSIVE Y CSS

## Propósito

Definir el procedimiento para conseguir que las webs construidas con Kadence funcionen correctamente en escritorio, tablet y móvil, utilizando primero las herramientas nativas y recurriendo a CSS solo cuando sea necesario.

---

## 1. PRIORIDAD DE CONFIGURACIÓN

Antes de escribir CSS, comprobar siempre:

1. WordPress.
2. Kadence.
3. Kadence Blocks.
4. Configuración responsive del bloque.
5. Plugin gratuito compatible.
6. CSS personalizado.
7. Código personalizado únicamente si no existe otra solución viable.

---

## 2. DISPOSITIVOS

Todo componente debe comprobarse como mínimo en:

- escritorio;
- tablet;
- móvil.

No considerar terminada una sección hasta comprobar las tres vistas.

---

## 3. PROPIEDADES RESPONSIVE

Para cada elemento comprobar, cuando corresponda:

- ancho;
- alto;
- max-width;
- padding;
- margin;
- tamaño de fuente;
- altura de línea;
- columnas;
- gutter;
- alineación;
- posición;
- visibilidad;
- orden;
- tamaño de imagen;
- botones.

---

## 4. ROW LAYOUT RESPONSIVE

Para las secciones construidas con Row Layout documentar:

### Escritorio

Número de columnas y ancho.

### Tablet

Número de columnas y ancho.

### Móvil

Número de columnas y ancho.

Ejemplo:

```text
Desktop → 3 columnas
Tablet  → 2 columnas
Móvil   → 1 columna

El valor final dependerá del diseño.


---

5. TIPOGRAFÍA RESPONSIVE

Los títulos deben adaptarse al tamaño de pantalla.

Ejemplo orientativo:

H1
Desktop → 56px
Tablet  → 44px
Móvil   → 36px

No aplicar estos valores automáticamente.

Determinar los tamaños según el diseño y documentarlos.


---

6. ESPACIADO RESPONSIVE

Evitar mantener grandes paddings de escritorio en móvil.

Ejemplo:

Desktop → 80px
Tablet  → 56px
Móvil   → 32px

Los valores finales deben definirse según cada sección.


---

7. BOTONES RESPONSIVE

Comprobar:

tamaño;

padding;

ancho;

alineación;

separación entre botones;

salto de línea;

comportamiento en móvil.


Cuando dos botones estén juntos en escritorio, comprobar si deben apilarse en móvil.


---

8. IMÁGENES RESPONSIVE

Comprobar:

proporción;

tamaño;

recorte;

posición;

resolución;

carga;

visualización móvil.


No utilizar imágenes excesivamente grandes para móviles.


---

9. HEADER RESPONSIVE

Comprobar específicamente:

logo;

menú;

menú hamburguesa;

submenús;

CTA;

altura;

padding;

sticky;

alineación.


El header debe ser funcional y visualmente coherente en todos los dispositivos.


---

10. FOOTER RESPONSIVE

Comprobar:

columnas;

orden;

enlaces;

texto;

iconos;

padding;

alineación.


Las columnas normalmente deben reorganizarse en móvil.


---

11. CSS PERSONALIZADO

Utilizar CSS únicamente cuando no exista una solución adecuada mediante la configuración disponible.

Antes de escribir CSS preguntar:

> ¿Esto puede hacerse mediante Kadence?



Si la respuesta es sí:

No utilizar CSS.


---

12. CSS AISLADO

Cuando sea necesario CSS, debe afectar únicamente al elemento previsto.

Evitar selectores demasiado generales como:

h2 {
}

cuando puedan afectar a toda la web.

Preferir clases específicas.

Ejemplo:

.mi-componente h2 {
}


---

13. CSS RESPONSIVE

Cuando un cambio sea específico de un dispositivo, utilizar media queries.

Ejemplo:

@media (max-width: 768px) {
    .mi-componente {
        /* ajuste móvil */
    }
}

Los breakpoints exactos deben adaptarse a los controles y breakpoints utilizados por el proyecto.

No asumir que todos los proyectos utilizan los mismos puntos de ruptura.


---

14. CSS Y PRIORIDAD

No utilizar !important por defecto.

Solo utilizarlo cuando exista un conflicto de especificidad real y se haya comprobado que no existe una solución mejor.


---

15. CSS DOCUMENTADO

Todo CSS incorporado debe registrar:

objetivo;

elemento afectado;

motivo;

ubicación;

dispositivos afectados;

posible conflicto;

fecha o versión si resulta relevante.



---

16. VALIDACIÓN VISUAL

Después de cualquier cambio responsive:

1. comprobar escritorio;


2. comprobar tablet;


3. comprobar móvil;


4. comprobar diferentes anchos de pantalla;


5. comprobar textos largos;


6. comprobar botones;


7. comprobar imágenes;


8. comprobar navegación.




---

17. PROBLEMAS HABITUALES

Registrar progresivamente soluciones para:

desbordamiento horizontal;

textos demasiado grandes;

columnas que no se apilan correctamente;

botones que se salen de pantalla;

imágenes deformadas;

padding excesivo;

márgenes inesperados;

header demasiado alto;

menú móvil incorrecto;

footer desordenado;

CSS heredado;

conflictos entre bloques.



---

18. NO SOLUCIONAR CON CSS A CIEGAS

Si algo no aparece correctamente:

1. identificar el elemento;


2. comprobar qué bloque lo genera;


3. comprobar sus opciones;


4. comprobar estilos globales;


5. comprobar estilos heredados;


6. comprobar responsive;


7. comprobar CSS existente;


8. solo entonces añadir o modificar CSS.




---

19. PRUEBA FINAL

Antes de considerar terminada una web:

Desktop

[ ] Layout correcto

[ ] Tipografía correcta

[ ] Espaciado correcto

[ ] Imágenes correctas

[ ] Botones correctos

[ ] Header correcto

[ ] Footer correcto


Tablet

[ ] Layout correcto

[ ] Tipografía correcta

[ ] Espaciado correcto

[ ] Imágenes correctas

[ ] Botones correctos

[ ] Navegación correcta


Móvil

[ ] Sin scroll horizontal

[ ] Layout correcto

[ ] Tipografía correcta

[ ] Espaciado correcto

[ ] Imágenes correctas

[ ] Botones correctos

[ ] Menú correcto

[ ] Footer correcto



---

20. REGLA OPERATIVA

Cuando el usuario tenga que modificar un elemento responsive, las instrucciones deberán indicar:

OBJETIVO

Qué queremos conseguir.

RUTA

Dónde entrar.

ELEMENTO

Qué bloque seleccionar.

OPCIÓN

Qué control modificar.

DESKTOP

Valor.

TABLET

Valor.

MÓVIL

Valor.

VERIFICACIÓN

Qué debe aparecer después.


---

21. REGLA FINAL

Una web no se considera terminada porque funcione en escritorio.

Se considera terminada cuando:

funciona + se ve correctamente + es usable + mantiene coherencia visual en escritorio, tablet y móvil.
