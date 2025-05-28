
Poner width: 100vw y height: 100vh en el body hace que el cuerpo de la página ocupe todo el ancho y alto de la ventana del navegador, sin importar el contenido interno.

¿Por qué es conveniente?
Diseño de pantalla completa: Es útil para layouts modernos donde quieres que el fondo, imágenes o secciones ocupen toda la pantalla, incluso si el contenido es menor.
Fondos y secciones: Permite aplicar fondos, imágenes o colores que cubran toda la ventana.
Centrado vertical y horizontal: Facilita el uso de Flexbox o Grid para centrar elementos en toda la pantalla.
Landing pages y hero sections: Muy usado en páginas de inicio donde el primer bloque debe ocupar toda la vista del usuario.

Precaución
Puede causar scroll horizontal si hay elementos con margen/padding o si el contenido se desborda, por eso se suele usar también overflow-x: hidden;.
En resumen:
Te da control total sobre el área visible del navegador, ideal para diseños modernos y responsivos.


margin-inline-end
¿Para qué se usa?
margin-inline-end agrega un margen en el extremo "final" del eje horizontal, según la dirección de escritura del texto (por ejemplo, a la derecha en idiomas de izquierda a derecha como el español o inglés).
Ventaja:
Es útil para diseños internacionales, ya que si el idioma cambia a uno de derecha a izquierda (como árabe o hebreo), el margen se aplicará automáticamente al otro lado.
Ejemplo:

.icono {
    margin-inline-end: 8px;
}

Esto agrega un margen a la derecha en español/inglés, o a la izquierda en árabe.
vertical-align: middle
¿Para qué se usa?
vertical-align: middle alinea verticalmente un elemento en línea (inline o inline-block), como imágenes o iconos, respecto a la línea base del texto circundante.
Uso típico:
Se usa para que iconos o imágenes queden centrados verticalmente respecto al texto con el que están alineados.
Ejemplo:
Así, el icono se verá alineado al centro de la altura de la línea de texto.
Resumen:

margin-inline-end: margen adaptable al final del eje horizontal, útil para soportar varios idiomas.

vertical-align: middle: centra verticalmente elementos inline respecto al texto.



/*flex-grow es una propiedad en CSS utilizada en el contexto de Flexbox, un modelo de layout que permite distribuir el espacio entre los elementos de una manera más eficiente y adaptable.*/
/*
Qué hace flex-grow: 1?
flex-grow define cómo se distribuirá el espacio disponible entre los elementos flexibles dentro de un contenedor flex. Es decir, controla si un elemento puede crecer para ocupar espacio sobrante en el contenedor.

Si flex-grow está establecido en 1, el elemento puede crecer para llenar el espacio disponible en el contenedor. Por ejemplo:

Si hay múltiples elementos en un contenedor flex y todos tienen flex-grow: 1, el espacio disponible se dividirá de manera equitativa entre ellos.
Si un elemento tiene flex-grow: 2 y otro tiene flex-grow: 1, el primer elemento ocupará el doble de espacio que el segundo.
Ejemplo simple
*/