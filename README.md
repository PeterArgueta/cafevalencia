# Café Valencia

Sitio estático de Café Valencia, Jutiapa, Guatemala. HTML, CSS y JavaScript sin compilación ni dependencias de ejecución.

## Archivos

- `index.html`: información comercial, secciones y enlaces de pedido por WhatsApp.
- `assets/styles.css`: paleta, tipografías, componentes y reglas responsive.
- `assets/site.js`: menú móvil accesible. Sin JavaScript, el menú permanece visible.
- `assets/fonts/`: Lato y Playfair Display, con sus respectivas licencias OFL.
- `images/`: fotografías reales del producto en WebP de 480 y 960 px para portada y catálogo; las seis imágenes anteriores se conservan como archivos. Las secciones informativas y la galería usan las tres fotografías reales de la finca proporcionadas por la marca, optimizadas a 360 y 717 px.

## Vista local

Desde la raíz del proyecto:

```sh
python3 -m http.server 8000
```

Abrir `http://localhost:8000`. No se requiere instalar paquetes ni ejecutar un build.

## Publicación y mantenimiento

Los recursos usan rutas relativas compatibles con GitHub Pages bajo `/cafevalencia/`. Revisar los cambios en una rama y un pull request antes de incorporarlos a la rama publicada.

Al actualizar contenido comercial, confirmar precio, presentación, disponibilidad, características y contacto con la marca. Las fotografías deben corresponder al producto y a la finca; no generar sustitutos con IA.

Cuando se reciban las fotografías originales, preparar versiones optimizadas para web, actualizar sus dimensiones y descripciones, y conservar la prioridad de carga de la portada y la carga diferida del resto.

Las fotos del producto corresponden a `283379.jpg` (bolsa en mano) y `283321.jpg` (bolsa en mesa), proporcionadas por la marca. Solo se redimensionaron y comprimieron; no se generaron fondos ni se retocó el empaque o la etiqueta.

El catálogo aísla la bolsa con un `clipPath` SVG sobre la fotografía original. No reconstruye el empaque, el texto ni el código QR. La imagen de origen se conserva y el fondo marfil pertenece al diseño de la página. El recorte generado durante la exploración visual no se incorpora al sitio.

Fotos de finca: `293377.jpg` (rama), `293417.jpg` (frutos) y `293423.jpg` (cafetal). Se redimensionaron y comprimieron para web sin inventar elementos ni modificar su contenido.

## Tipografía

El sistema usa Altivo Regular (peso 400), con Lato Regular como alternativa temporal. Se retiraron el cambio de color y la cursiva dentro del título, y se redujeron las mayúsculas espaciadas y el énfasis decorativo.

Altivo solo se activa con `local()` cuando está instalada en el dispositivo. Para servirla a todos los visitantes falta incorporar un WOFF2 autorizado para web o un Web Project de Adobe Fonts proporcionado por la marca. No se descarga una copia de terceros ni se solicita un archivo inexistente. La vista de revisión utiliza Lato cuando Altivo no está disponible y no debe presentarse como una muestra real de Altivo.

La jerarquía depende del tamaño, interlineado y separación; no se simulan negritas ni cursivas de Altivo Regular. Los archivos de las tipografías anteriores se conservan, pero los estilos Playfair Display y Lato Bold ya no se cargan.
