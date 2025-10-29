
Proyecto Web --- Estilos CSS de Sitio de Videojuegos
Este proyecto consiste en un sitio web diseñado con HTML y CSS,
orientado a presentar juegos, géneros y formularios de contacto o
comunidad, con un diseño adaptable y moderno.

El sitio se organiza mediante CSS Grid, Flexbox y media
queries para asegurar una visualización óptima en distintas
resoluciones.

Estructura del Proyecto
El sitio cuenta con tres hojas de estilo principales:
1. style.css (principal de detalle del juego)

Define el diseño completo de las páginas de detalle o presentación
de un juego.
2. catalogo.css (catálogo o listado de juegos)

Gestiona la disposición de las imágenes por género y la navegación
lateral con categorías.
3. contacto.css (formulario de contacto o comunidad)

Aplica los estilos para la sección de contacto, formulario y
términos de servicio.

Estilos Generales
Todos los archivos comparten una base común:
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html, body {
  height: 100%;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  background-color: lightgreen;
  color: black;
}

Esto garantiza consistencia tipográfica, márgenes nulos y una paleta
verde clara coherente con la temática ecológica/natural del sitio.

Distribución Principal (grid-container)
Cada página utiliza un layout en cuadrícula (CSS Grid) para
organizar las áreas:
"header header"
"aside main"
"footer footer"
* Header: Barra superior con logotipo, buscador y enlaces
(comentarios / Steam).\
* Aside: Barra lateral de navegación con categorías y enlaces.\
* Main: Contenido principal (ya sean juegos, descripciones o
formularios).\
* Footer: Pie de página con créditos y enlaces a la comunidad.

style.css -- Página de Detalle del Juego
* Contiene clases como .portada, .info-juego, .texto-juego y
.bloque-info para mostrar información detallada sobre un
videojuego.\
* Incluye efectos de hover con scale y transition para
imágenes y botones.\
* Usa una estructura tipo "panel" con fondo blanco semitransparente
sobre verde.\
* Totalmente responsive, ajustándose a pantallas menores a 900 px
y 550 px.
catalogo.css -- Página de Catálogo de Juegos
* Presenta imágenes por géneros dentro de contenedores
.imagenes-row.\
* Usa flex-wrap para que las imágenes se reorganicen
automáticamente.\
* Las categorías del sidebar (.categoria) y los enlaces (.link)
facilitan la navegación.\
* Añade sombras, bordes redondeados y efectos de escala al pasar el
cursor.\
* Estructura de color coherente con la del resto del sitio: tonos
verdes y grises.
contacto.css -- Página de Contacto / Comunidad
* Diseña el formulario de contacto dentro de .contenedor,
dividido en dos columnas:
	* Columna izquierda: formulario (.formulario)\
	* Columna derecha: términos o información adicional (.terminos)\
* Uso de inputs, textarea y checkboxes estilizados.\
* Botones .cancel (rojo) y .submit (azul) con bordes redondeados.\
* El header y footer mantienen coherencia visual con las demás
páginas.\
* Uso de position: sticky; en el header para mantenerlo visible al
hacer scroll.

Tecnologías Usadas
* HTML5 para la estructura de contenido.\
* CSS3 con:
	* Grid Layout para la estructura global.\
	* Flexbox para la alineación y distribución interna.\
	* Media Queries para la adaptabilidad.\
	* Transiciones y transformaciones (scale, translateY,
hover).

Cómo Visualizar el Proyecto
1. Clona o descarga el repositorio.\
2. Abre cualquiera de los archivos HTML correspondientes en tu
navegador:
	* index.html → catálogo de juegos\
	* juego.html → detalle del juego\
	* contacto.html → formulario de contacto\
3. Asegúrate de tener los tres CSS vinculados correctamente mediante
etiquetas <link> en cada página.

Créditos
* Autores: Marcos Adam Martínez Ouhabi y Aitor Coscollano Vélez
* Tema visual: verde claro con estructura modular responsiva.
