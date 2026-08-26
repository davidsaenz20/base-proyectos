04-BLOQUES-Y-COMPONENTES.md

# KADENCE — BLOQUES Y COMPONENTES

## Propósito

Documentar los bloques y componentes que utilizaremos para construir páginas profesionales con WordPress, Gutenberg y Kadence Blocks gratuito.

## 1. PRINCIPIO DE CONSTRUCCIÓN

Las páginas deben construirse utilizando componentes reutilizables siempre que sea posible.

Orden recomendado:

1. Sección.
2. Container / Row Layout.
3. Columnas.
4. Contenido.
5. Elementos visuales.
6. CTA.
7. Espaciado.
8. Responsive.
9. Validación.

---

## 2. BLOQUES PRIORITARIOS

La Knowledge Base debe documentar progresivamente los bloques gratuitos disponibles.

Prioridad inicial:

- Row Layout;
- Advanced Heading;
- Advanced Button;
- Info Box;
- Image;
- Icon;
- Icon List;
- Tabs;
- Accordion;
- Advanced Gallery;
- Testimonial;
- Form;
- Spacer.

La disponibilidad exacta debe verificarse según la versión instalada.

---

## 3. ROW LAYOUT

Es uno de los bloques principales de nuestra metodología.

Debe documentarse:

- columnas;
- ancho;
- max-width;
- gutter;
- padding;
- margin;
- background;
- imagen de fondo;
- overlay;
- min-height;
- alineación;
- alineación vertical;
- responsive;
- columnas por dispositivo;
- visibilidad responsive.

---

## 4. ADVANCED HEADING

Debe utilizarse para:

- títulos;
- subtítulos;
- encabezados de secciones;
- textos destacados.

Documentar:

- contenido;
- HTML heading;
- tipografía;
- tamaño;
- peso;
- color;
- alineación;
- margen;
- responsive;
- decoración;
- enlace si existe.

---

## 5. ADVANCED BUTTON

Debe utilizarse para CTA y acciones importantes.

Documentar:

- texto;
- URL;
- estilo;
- tamaño;
- padding;
- colores;
- borde;
- border-radius;
- hover;
- iconos;
- alineación;
- responsive.

Debe utilizar preferentemente el estilo global de botones.

---

## 6. INFO BOX

Puede utilizarse para:

- beneficios;
- servicios;
- características;
- ventajas;
- bloques informativos.

Documentar:

- icono;
- título;
- descripción;
- enlace;
- colores;
- tipografía;
- espaciado;
- fondo;
- borde;
- sombra;
- hover;
- responsive.

---

## 7. IMAGE

Documentar:

- tamaño;
- relación de aspecto;
- alineación;
- enlace;
- alt text;
- lazy loading;
- borde;
- border-radius;
- sombra;
- responsive.

Las imágenes deben optimizarse antes de incorporarlas.

---

## 8. ICON

Documentar:

- biblioteca;
- tamaño;
- color;
- alineación;
- espaciado;
- enlace;
- responsive.

Evitar utilizar iconos únicamente como decoración cuando puedan mejorar la comprensión.

---

## 9. ICON LIST

Puede utilizarse para:

- ventajas;
- características;
- listas de servicios;
- pasos;
- elementos destacados.

Documentar:

- icono;
- texto;
- separación;
- colores;
- tipografía;
- responsive.

---

## 10. TABS

Utilizar únicamente cuando dividir contenido en pestañas mejore realmente la experiencia.

Documentar:

- títulos;
- contenido;
- orientación;
- estilo;
- colores;
- tipografía;
- espaciado;
- responsive;
- accesibilidad.

No utilizar tabs para ocultar contenido importante que debería ser visible directamente.

---

## 11. ACCORDION

Puede utilizarse especialmente para FAQ.

Documentar:

- título;
- contenido;
- iconos;
- apertura inicial;
- colores;
- tipografía;
- bordes;
- espaciado;
- responsive.

---

## 12. TESTIMONIAL

Documentar:

- nombre;
- fotografía;
- cargo;
- valoración;
- texto;
- diseño;
- tipografía;
- colores;
- responsive.

Los testimonios deben ser reales cuando el proyecto pase a producción.

---

## 13. FORMULARIOS

Antes de crear un formulario comprobar si:

- WordPress puede resolverlo;
- Kadence Blocks puede resolverlo;
- existe un plugin gratuito adecuado.

Documentar:

- campos;
- etiquetas;
- placeholders;
- validación;
- mensajes;
- email;
- protección antispam;
- responsive;
- integración con n8n si procede.

---

## 14. COMPONENTES REUTILIZABLES

Siempre que un elemento se repita en varias páginas, estudiar si debe convertirse en componente reutilizable.

Ejemplos:

- CTA;
- tarjeta de servicio;
- bloque de contacto;
- FAQ;
- testimonial;
- bloque de beneficios;
- navegación contextual.

---

## 15. TARJETAS

Para cada tarjeta documentar:

- container;
- imagen;
- icono;
- título;
- texto;
- botón;
- padding;
- margen;
- borde;
- radius;
- sombra;
- hover;
- responsive.

Las tarjetas de una misma sección deben compartir estructura.

---

## 16. SECCIONES

Una sección debe tener una función clara.

Ejemplos:

- Hero;
- Beneficios;
- Servicios;
- Problema;
- Solución;
- Proceso;
- Testimonios;
- FAQ;
- CTA;
- Contacto.

Evitar crear secciones únicamente para llenar espacio.

---

## 17. SISTEMA DE ESPACIADO

Mantener una escala coherente.

Ejemplo orientativo:

```text
XS = 8px
S  = 16px
M  = 24px
L  = 40px
XL = 64px
XXL = 96px

Los valores pueden modificarse según el diseño del proyecto.


---

18. RESPONSIVE

Cada componente debe comprobarse en:

escritorio;

tablet;

móvil.


Documentar qué controles de Kadence permiten modificar:

tamaño;

padding;

margin;

columnas;

alineación;

visibilidad;

orden.



---

19. CSS

Antes de utilizar CSS:

1. comprobar opciones del bloque;


2. comprobar opciones globales;


3. comprobar Kadence;


4. comprobar Gutenberg;


5. comprobar plugin gratuito.



Solo utilizar CSS cuando sea necesario.


---

20. INSTRUCCIONES OPERATIVAS

Cada componente documentado deberá permitir generar instrucciones como:

OBJETIVO

Crear una sección de tres tarjetas.

BLOQUE

Row Layout.

CONFIGURACIÓN

3 columnas en escritorio.

2 columnas en tablet.

1 columna en móvil.

ESTILO

Utilizar estilos globales.

VERIFICACIÓN

Comprobar alineación, espaciado y responsive.


---

21. REGISTRO DE NUEVOS COMPONENTES

Cuando durante un proyecto se cree un componente reutilizable:

1. definir su función;


2. documentar su estructura;


3. documentar su configuración;


4. documentar responsive;


5. documentar CSS si existe;


6. registrar la solución;


7. evaluar su reutilización futura.




---

Regla final

El objetivo no es utilizar todos los bloques disponibles.

El objetivo es disponer de un conjunto pequeño de componentes fiables que permitan construir webs diferentes, profesionales, coherentes y fáciles de mantener.

