02-CONFIGURACION-GLOBAL.md

# KADENCE — CONFIGURACIÓN GLOBAL

## Propósito

Este documento define cómo configurar los elementos globales de Kadence para que todas las páginas de un proyecto mantengan una apariencia coherente.

La prioridad es configurar primero los elementos globales y después construir las páginas individuales.

---

## 1. PRINCIPIO GLOBAL

Antes de diseñar una página individual se debe definir:

- colores;
- tipografías;
- tamaños de títulos;
- botones;
- ancho del contenido;
- espaciados;
- enlaces;
- estructura general;
- comportamiento responsive.

No se deben configurar estos elementos manualmente en cada bloque cuando puedan establecerse globalmente.

---

## 2. COLORES GLOBALES

Crear una paleta coherente para cada proyecto.

Debe contemplar como mínimo:

- color principal;
- color secundario;
- color de acento;
- color de texto;
- color de texto secundario;
- color de fondo principal;
- color de fondo alternativo;
- color de borde;
- color de enlace;
- color hover.

Los valores concretos se decidirán según el diseño del proyecto.

### Regla

Los bloques deben utilizar preferentemente los colores globales definidos.

Evitar introducir colores personalizados sin motivo.

---

## 3. TIPOGRAFÍA GLOBAL

Definir como mínimo:

- fuente principal;
- fuente secundaria si fuera necesaria;
- H1;
- H2;
- H3;
- H4;
- H5;
- H6;
- texto normal;
- enlaces;
- botones.

Para cada nivel documentar:

- familia tipográfica;
- peso;
- tamaño;
- altura de línea;
- espaciado entre letras;
- tamaño en escritorio;
- tamaño en tablet;
- tamaño en móvil.

---

## 4. ESCALA TIPOGRÁFICA

Siempre que sea posible utilizar una escala coherente.

Ejemplo orientativo:

- H1: 48–64 px;
- H2: 36–48 px;
- H3: 28–36 px;
- H4: 22–28 px;
- texto: 16–18 px;
- texto pequeño: 14–16 px.

Estos valores son orientativos.

No deben copiarse automáticamente a todos los proyectos.

La escala final debe adaptarse al diseño.

---

## 5. ANCHO GLOBAL

Definir un ancho máximo para el contenido principal.

Como referencia inicial:

- contenido estándar: aproximadamente 1100–1200 px;
- contenido amplio: aproximadamente 1200–1400 px.

El valor final dependerá del proyecto.

Debe mantenerse una estructura consistente entre páginas.

---

## 6. ESPACIADO

Definir una lógica de espaciado reutilizable.

Debe contemplar:

- separación entre secciones;
- padding superior;
- padding inferior;
- separación entre títulos y textos;
- separación entre textos y botones;
- separación entre columnas;
- separación entre tarjetas.

Evitar utilizar valores arbitrarios diferentes en cada bloque.

---

## 7. BOTONES

Definir globalmente:

- tipografía;
- tamaño;
- peso;
- padding;
- border-radius;
- borde;
- color de fondo;
- color del texto;
- hover;
- transición;
- comportamiento responsive.

Cuando existan botones secundarios, definir también su estilo.

---

## 8. ENLACES

Definir:

- color;
- hover;
- subrayado;
- transición.

Los enlaces de navegación pueden tener un comportamiento diferente de los enlaces del contenido.

Documentar ambas configuraciones cuando sea necesario.

---

## 9. HEADER

El header debe configurarse globalmente antes de crear las páginas.

Definir:

- logo;
- altura;
- estructura;
- navegación;
- botón CTA;
- colores;
- tipografía;
- espaciado;
- comportamiento sticky si se utiliza;
- versión móvil.

La configuración detallada se documentará en:

`03-HEADER-FOOTER-MENUS.md`

---

## 10. FOOTER

Definir globalmente:

- estructura;
- columnas;
- navegación;
- información de contacto;
- redes sociales;
- copyright;
- colores;
- tipografía;
- espaciado;
- responsive.

La configuración detallada se documentará en:

`03-HEADER-FOOTER-MENUS.md`

---

## 11. RESPONSIVE

Todo elemento global debe comprobarse en:

- escritorio;
- tablet;
- móvil.

No asumir que un diseño correcto en escritorio funcionará automáticamente en móvil.

Especial atención a:

- H1;
- H2;
- navegación;
- botones;
- padding;
- márgenes;
- columnas;
- imágenes;
- header;
- footer.

---

## 12. REGLA MOBILE FIRST EN LA VALIDACIÓN

Aunque la construcción pueda comenzar desde escritorio, siempre se debe comprobar el resultado móvil.

La validación mínima será:

1. escritorio;
2. tablet;
3. móvil.

Si existe una propiedad responsive específica de Kadence, utilizarla antes que CSS personalizado.

---

## 13. CSS GLOBAL

El CSS personalizado debe utilizarse únicamente cuando no exista una solución adecuada mediante:

1. WordPress;
2. Kadence;
3. Kadence Blocks;
4. plugin gratuito.

Cuando sea necesario utilizar CSS:

- documentar el motivo;
- documentar dónde se coloca;
- documentar a qué elementos afecta;
- documentar si afecta a responsive;
- evitar selectores excesivamente genéricos;
- evitar CSS que pueda romper otros componentes.

---

## 14. CONFIGURACIÓN POR PROYECTO

Cada proyecto deberá definir sus propios valores globales.

Ejemplo:

### Colores

```text
Primario:
#XXXXXX

Secundario:
#XXXXXX

Acento:
#XXXXXX

Texto:
#XXXXXX

Fondo:
#XXXXXX

Tipografía

Principal:
[Fuente]

H1:
[Tamaño / peso / línea]

H2:
[Tamaño / peso / línea]

H3:
[Tamaño / peso / línea]

Body:
[Tamaño / peso / línea]

Layout

Container:
[Valor]

Sección:
[Padding]

Gutter:
[Valor]

Estos valores deben quedar registrados en la documentación específica del proyecto.


---

15. VERIFICACIÓN

Después de configurar los elementos globales comprobar:

todas las páginas utilizan la tipografía correcta;

los colores globales funcionan;

los botones mantienen coherencia;

los enlaces funcionan correctamente;

el ancho de contenido es consistente;

el header es correcto;

el footer es correcto;

el diseño funciona en móvil;

no existen estilos heredados inesperados.



---

16. REGLA DE NO DUPLICACIÓN

No crear estilos independientes para elementos que deberían compartir estilo global.

Ejemplo incorrecto:

Botón página A → azul
Botón página B → azul
Botón página C → azul

Si todos deben ser iguales, debe existir un estilo global.

Ejemplo correcto:

Estilo global:
Botón primario

Página A → usa estilo global
Página B → usa estilo global
Página C → usa estilo global


---

17. ACTUALIZACIÓN DE LA DOCUMENTACIÓN

Cuando se descubra una configuración útil durante un proyecto:

1. comprobar que funciona;


2. documentar la ruta exacta;


3. documentar la opción;


4. documentar el valor;


5. indicar la versión cuando sea relevante;


6. añadir la solución al documento correspondiente.



La Knowledge Base debe mejorar con cada proyecto.


---

18. REGLA FUNDAMENTAL

Primero:

CONFIGURACIÓN GLOBAL

Después:

COMPONENTES REUTILIZABLES

Después:

PÁGINAS

Después:

AJUSTES ESPECÍFICOS

Y solamente al final:

CSS/CÓDIGO ESPECÍFICO

El objetivo es conseguir una web visualmente coherente utilizando el menor nivel razonable de complejidad.


