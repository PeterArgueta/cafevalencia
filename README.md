# Café Valencia

Sitio estático de Café Valencia, Jutiapa, Guatemala. HTML, CSS y JavaScript sin compilación ni dependencias de ejecución.

## Archivos

- `index.html`: información comercial, secciones y enlaces de pedido por WhatsApp.
- `assets/styles.css`: paleta, tipografías, componentes y reglas responsive.
- `assets/site.js`: menú móvil accesible. Sin JavaScript, el menú permanece visible.
- `assets/fonts/`: Lato y Playfair Display, con sus respectivas licencias OFL.
- `images/`: seis imágenes existentes, conservadas hasta recibir fotografías reales aprobadas.

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
