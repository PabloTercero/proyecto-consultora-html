# Práctica Final: Sitio Web PT Consultorías

Este es el repositorio con mi proyecto para la práctica intermodular de HTML y CSS. Se trata de la web corporativa para una empresa ficticia llamada **PT Consultorías**, especializada en auditorías tecnológicas.

## Estructura de archivos

He organizado el proyecto siguiendo las instrucciones del enuncido:
* **`/css`**: Aquí está la hoja de estilos única (`style.css`).
* **`/img`**: Contiene el logo, el favicon y las imágenes de fondo y producto.
* **Archivos HTML**: He creado los 4 archivos obligatorios (`index`, `proyecto-reservas`, `cronologia` y `contacto`).

## Diseño y decisiones tomadas

Para el diseño he intentado que parezca una empresa seria y tecnológica:

**Colores:** He usado variables CSS (`:root`) para definir un azul principal (`#0056b3`) y gris oscuro, así si hay que cambiar el color se cambia en todo a la vez.
**Tipografía:** He importado la fuente **Roboto** desde Google Fonts para cumplir con el requisito del Hito 1[cite: 143].
**Unidades:** He tenido cuidado de usar **`rem`** para los tamaños de fuente y márgenes, y así evitar la penalización por usar píxeles.

## Dificultades encontradas y soluciones

Durante la práctica me encontré con algunos problemas que he ido solucionando:

1.  **El Layout de 2 columnas:** En la página de "Servicios" (`proyecto-reservas.html`), me costó que la barra lateral (`aside`) se quedara fija y el contenido (`main`) ocupara el resto.Lo solucioné usando **Flexbox** en el contenedor padre y poniéndole `flex-grow: 1` a la parte principal.

2.  **El Menú en el móvil:** Al principio, al reducir la pantalla, el menú se rompía. [cite_start]He añadido una **Media Query** (`max-width: 768px`) para cambiar la dirección del flex a `column` y que se vea bien en vertical.

3.  **Formulario sobre el fondo:** El texto del formulario no se leía bien sobre la imagen de fondo. Lo arreglé poniendo un color de fondo blanco con transparencia (`rgba`) para que hiciera contraste.



