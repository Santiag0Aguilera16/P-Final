Cuchillería Artesanal Osvaldo Aguilera - Sitio Web
Descripción
Este proyecto es un sitio web para la Cuchillería Artesanal Osvaldo Aguilera, dedicado a mostrar los trabajos personalizados y hechos a mano por el artesano Osvaldo Aguilera. El sitio web tiene cinco secciones principales: Inicio, Servicios, Taller, Galería, y Contacto. Está diseñado con HTML5, SCSS, y Bootstrap para lograr un diseño moderno, responsive y bien estructurado.

Estructura del Proyecto
La estructura del proyecto sigue una organización en carpetas que permite un desarrollo ordenado y una fácil escalabilidad.

Carpetas Principales
/css - Contiene los archivos CSS generados por SCSS.
/scss - Contiene los archivos SCSS organizados en partials.
/images - Carpeta con todas las imágenes utilizadas en el proyecto.
/pages - Archivos HTML correspondientes a cada sección del sitio web.
Secciones del Sitio
Inicio
Contiene una breve introducción a la cuchillería y un botón de "Ver más" que enlaza a otras secciones del sitio.
El estilo del botón está gestionado con un partial específico para botones en SCSS.
Servicios
Describe los servicios ofrecidos por la cuchillería.
Incluye un botón "Ver más" que enlaza a la página del taller.
Estilo del botón consistente con otras secciones del sitio.
Taller
Explicación detallada del taller y el proceso de creación artesanal.
Compatible con Bootstrap y Flexbox para garantizar una disposición responsive.
Galería
Presenta un carrusel de imágenes con algunos de los trabajos destacados.
El carrusel está hecho con Bootstrap, y las imágenes se ajustan para que no ocupen demasiado espacio y se adapten a la vista.
La galería es totalmente compatible con SCSS para facilitar futuros cambios.
Contacto
Formulario de contacto y datos para que los clientes puedan ponerse en contacto con Osvaldo Aguilera.
Se ha implementado un layout basado en Bootstrap y Flexbox para asegurar una buena presentación.
Incluye una lista de redes sociales.
Instalación y Configuración
Clona este repositorio en tu máquina local:

bash
Copiar código
git clone https://github.com/usuario/cuchilleria-artesanal.git
Asegúrate de tener instalado Node.js y SCSS. Si no tienes SCSS, instálalo globalmente:

bash
Copiar código
npm install -g sass
Compila los archivos SCSS en CSS:

bash
Copiar código
sass --watch scss:css
Abre index.html en tu navegador para ver el sitio.

Estructura SCSS
La estructura SCSS está organizada de manera modular utilizando partials, variables, mixins y nesting para optimizar el mantenimiento del código.

Archivos SCSS:
_variables.scss: Aquí están definidas todas las variables globales de colores, tipografías y tamaños de fuente.
_mixins.scss: Incluye mixins para reutilización de estilos como Flexbox y media queries.
_base.scss: Contiene los estilos base y los reseteos necesarios para asegurar consistencia entre navegadores.
_header.scss: Estilos específicos para la barra de navegación y el header del sitio.
_inicio.scss: Estilos para la sección de inicio.
_servicios.scss: Estilos para la sección de servicios.
_taller.scss: Estilos para la sección del taller.
_galeria.scss: Estilos para la galería y el carrusel de imágenes.
_contacto.scss: Estilos para la sección de contacto, implementando Bootstrap y Flexbox.
_buttons.scss: Estilos centralizados para los botones "Ver más" en todas las secciones.
El archivo principal style.scss se encarga de importar todos los partials SCSS.

Ejemplo de Importación en style.scss:
scss
Copiar código
@import 'variables';
@import 'mixins';
@import 'base';
@import 'header';
@import 'inicio';
@import 'servicios';
@import 'taller';
@import 'galeria';
@import 'contacto';
@import 'buttons';
Características
Responsive Design: El sitio es totalmente responsive y se ajusta a diferentes tamaños de pantalla utilizando Bootstrap y media queries personalizadas en SCSS.
Bootstrap: Se utiliza la última versión de Bootstrap (v5.3.3) para la estructuración del carrusel de la galería, el sistema grid, y algunos estilos de formularios.
SCSS Modular: Todos los estilos están organizados de manera modular utilizando SCSS para una fácil personalización y escalabilidad.
Carrusel Adaptable: El carrusel en la galería ajusta su tamaño según el viewport, y las imágenes se adaptan sin distorsionarse.
Problemas Resueltos
Formulario de Contacto con Bootstrap y Flexbox: Se ajustó la estructura del formulario de contacto para ser compatible con SCSS y utilizar Bootstrap para el diseño responsivo.
Carrusel en Galería: El carrusel ocupaba demasiado espacio. Se corrigió el tamaño y la adaptación de las imágenes utilizando Bootstrap y SCSS.
Botones "Ver más": Se resolvieron problemas de posicionamiento inconsistente en las diferentes secciones mediante la centralización de estilos en un partial SCSS.
Licencia
Este proyecto está licenciado bajo la MIT License.
