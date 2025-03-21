# BetterIfYouDoNotReadme.md

## Descripción General

Esta guía de estilos describe el marco visual y técnico utilizado en el proyecto del portfolio de **José Braulio Palomo Vázquez**. Aquí se detallan la paleta de colores, las tipografías, el logo personal, las librerías empleadas, enlaces de referencia a webs utilizadas para obtener código y los problemas técnicos encontrados durante el desarrollo, junto con sus soluciones.

## Paleta de Colores

- **Fondo:**  
  - Color principal: `#000000` (negro)

- **Texto y Encabezados:**  
  - Texto de párrafos: `#ffffff` (blanco)  
  - Encabezados (por ejemplo, `<h3>`): `rgb(250, 250, 114)` (amarillo brillante)  
  - Enlaces del menú de navegación:  
    - Estado normal: `rgb(171, 196, 255)`  
    - Al pasar el ratón (hover): `rgb(223, 229, 243)`

- **Bordes y Acabados:**  
  - Bordes de la navegación: `rgb(235, 180, 200)` (punteado)  
  - Bordes en secciones específicas (por ejemplo, en la sección Skills) se utilizan colores semi-transparentes, como `rgba(22, 68, 160, 0.787)` y `rgba(216, 49, 49, 0.787)`.

## Tipografía

- **Fuentes Principales:**  
  - **"Press Start 2P"**  
  - **"Arvo"**  
  - **"Varela Round"**

- **Importación:**  
  Estas fuentes se importan desde [Google Fonts](https://fonts.google.com) utilizando la siguiente URL:

- La fuente de respaldo es `system-ui`.

## Estructura y Distribución

- **Contenedor Principal (Grid):**  
Se utiliza el contenedor `#grid-container` para dividir la página en tres áreas principales:
- **Header:** Encabezado con título personal, menú de navegación (con atributos `aria-label`) y una imagen animada (logo o gif).
- **Main:** Contenido principal dividido en secciones como "Who Am I?", "Skills" y "Curriculum", cada una con animaciones CSS definidas por keyframes.
- **Footer:** Pie de página que se muestra en todas las páginas, incluye el logo y los créditos.

- **Diseño Responsive:**  
Se emplean media queries para adaptar la distribución a distintos tamaños de pantalla.  
- En pantallas anchas (min-width: 1024px), el layout se redefine mediante el `#grid-container` y se ajustan los tamaños de imagen para evitar que sean excesivos.

## Logo Personal

- **Uso:**  
El logo se utiliza como favicon y se muestra también en el pie de página.

![Logo](img/favicon.png)

## Librerías y Referencias

- **Google Fonts:**  
- [Press Start 2P](https://fonts.google.com/specimen/Press+Start+2P)  
- [Arvo](https://fonts.google.com/specimen/Arvo)  
- [Varela Round](https://fonts.google.com/specimen/Varela+Round)

- **Referencias Externas:**  
- [MDN Web Docs](https://developer.mozilla.org)  
- [W3C HTML Validator](https://validator.w3.org/)

## Problemas Técnicos y Soluciones

- **Ajustes en el Diseño Responsive:**  
- **Problema:** He intentado hacer un carrusel de imágenes en la sección "About me".  
- **Solución:**  
  Busqué por internet una forma de hacerlo solo con CSS y en esta página encontré una [solución aceptable](https://www.enmilocalfunciona.io/crear-un-carrusel-de-imagenes-solo-con-css/)

- **Uso Exclusivo del Grid-Container en Vistas Anchas:**  
- **Problema:** Difucultad para manejar el sonido a mi antojo.  
- **Solución:** He incluido un poco de js para solucionar el problema con el control del sonido.

- **Escalado de Imágenes:**  
- **Problema:** En pantallas anchas, algunas imágenes resultaban demasiado grandes.  
- **Solución:** He ajustado las imágenes para mantener la cohesión visual.

- **Mejoras en Accesibilidad:**  
- Se añadieron atributos `aria-label` en los enlaces de navegación para mejorar la usabilidad en dispositivos de asistencia.

