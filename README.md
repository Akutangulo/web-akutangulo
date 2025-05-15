# Página web de Akutangulo.com
---
## Akutangulo Header

Este proyecto contiene el código para el encabezado (header) de la página web de **Akutangulo**, diseñado con un efecto visual animado en 3D para el logotipo. Incluye animaciones de "wobble" y "glow" para un impacto visual dinámico y atractivo.

### Descripción

El código crea un encabezado centrado con el texto "Akutangulo" repetido en múltiples capas `<h1>`, cada una con un desplazamiento en el eje Z para simular un efecto 3D. Las animaciones incluyen:

- **Wobble**: Una rotación 3D suave que da un efecto de balanceo continuo.
- **Glow**: Un cambio de color en la sombra del texto para un efecto de brillo dinámico.

El diseño es responsivo, ajustándose a diferentes tamaños de pantalla mediante `clamp` y media queries.

### Características

- **Animaciones CSS**: Efectos `wobble` y `glow` para un logotipo dinámico.
- **Diseño 3D**: Uso de `transform: translateZ` para crear capas superpuestas.
- **Responsividad**: Ajustes para pantallas pequeñas (≤768px).
- **Fuentes personalizadas**: Utiliza la fuente `bauhouse_akutangulo`.
- **Colores dinámicos**: Uso de la variable CSS `--color-akutangulo` para el color del texto.

### Requisitos

- Navegador web moderno compatible con animaciones CSS y transformaciones 3D.
- Archivos externos:
- Fuente personalizada `bauhouse_akutangulo`.

---
## **Div Mágico: Componente de Layout Responsivo Avanzado**

### Descripción General

El "Div Mágico" es un componente HTML/CSS altamente reutilizable diseñado para crear secciones de contenido visualmente atractivas y perfectamente adaptables. Su principal objetivo es presentar bloques de información compuestos por texto y un elemento multimedia (imagen, iframe o figura/diagrama) de forma dinámica y responsiva, resolviendo un desafío común: **lograr que la columna multimedia iguale automáticamente la altura de la columna de texto en pantallas grandes, sin importar el contenido.**

### Características Clave y Peculiaridades

Este componente destaca por las siguientes funcionalidades y técnicas:

1.  **Layout de Columnas Igualadas (Desktop):**
    *   En pantallas anchas (definido por media query, por defecto > 768px), el texto y el elemento multimedia se muestran en **dos columnas lado a lado**.
    *   **¡La Magia! Altura Automática Igualada:** El contenedor multimedia (`.imagen-magic-akutangulo`, `.iframe-magic-akutangulo`, `.figure-magic-akutangulo`) se estira **automáticamente** para tener exactamente la misma altura que el contenedor de texto (`.texto-magic-akutangulo`) hermano, gracias al uso inteligente de `display: flex` y `align-items: stretch` en el contenedor padre (`.contenido-bloque-magic`).
    *   **Solución Flexbox Avanzada:** Para que el *contenido* dentro del contenedor multimedia (específicamente `<img>` y `<figure>`) pueda usar `height: 100%` de forma fiable, se aplica una técnica peculiar pero efectiva: los propios contenedores `.imagen-magic-akutangulo` y `.figure-magic-akutangulo` se declaran también como `display: flex`. Esto establece un contexto de formato que permite al hijo calcular correctamente su altura porcentual respecto al contenedor estirado.
    *   **Iframes Absolutos:** Los `<iframe>` utilizan una estrategia diferente pero igualmente efectiva: `position: absolute` dentro de su contenedor (`.iframe-magic-akutangulo`), el cual es relativo y se estira con `align-self: stretch`.

2.  **Layout Alternante (Desktop):**
    *   El orden de las columnas (Texto-Multimedia o Multimedia-Texto) se controla fácilmente añadiendo las clases `bloque-normal-magic` o `bloque-reverse-magic` al contenedor `.contenido-bloque-magic`, utilizando `flex-direction: row` o `flex-direction: row-reverse`.

3.  **Apilamiento Vertical Fijo (Móvil):**
    *   En pantallas pequeñas (<= 768px), las columnas colapsan en una sola.
    *   **Orden Consistente:** Independientemente del orden en escritorio, en móvil el **texto (`.texto-magic-akutangulo`) SIEMPRE aparece primero (arriba)** y el **multimedia SIEMPRE aparece después (abajo)**. Esto se logra con la propiedad `order` de Flexbox (`order: 1` para texto, `order: 2` para multimedia) dentro de la media query, garantizando una lectura lógica y una alternancia visual (Texto, Media, Texto, Media...) en el flujo vertical.

4.  **Soporte Multimedia Flexible:**
    *   Diseñado para funcionar con:
        *   Imágenes (`<img>` dentro de `.imagen-magic-akutangulo`)
        *   Iframes (`<iframe>` dentro de `.iframe-magic-akutangulo`)
        *   Figuras/Diagramas (`<figure class="mermaid">` u otro contenido dentro de `.figure-magic-akutangulo`)

5.  **Optimización de Ancho de Texto:**
    *   En la vista de escritorio, el bloque de texto (`.texto-magic-akutangulo`) utiliza `flex-basis` (ej. `40%`) para sugerir un ancho inicial que favorezca la legibilidad, mientras que el bloque multimedia (`flex: 1`) ocupa el espacio restante.

6.  **CSS Enfocado y (Relativamente) Mínimo:**
    *   La solución se basa principalmente en CSS Flexbox y propiedades estándar.
    *   Se aplicaron modificaciones mínimas al CSS base original proporcionado para lograr la funcionalidad deseada, respetando la estructura HTML inicial.
    *   Se utiliza `box-sizing: border-box` para un manejo más predecible de padding y borders.

7.  **Personalización:**
    *   Fácilmente personalizable mediante variables CSS (si se definen externamente, como `--color-akutangulo`, `--color-texto`) y ajustando valores como `flex-basis`, `padding`, `margin` y el breakpoint de la media query.

Este componente soluciona de forma elegante el problema de las columnas de altura desigual en Flexbox, especialmente cuando una columna contiene imágenes o contenido dinámico que debe llenar el espacio vertical dictado por el texto, todo ello manteniendo un orden de apilamiento fijo y lógico en dispositivos móviles.

---

## Akutangulo Footer

Este proyecto contiene el código para el pie de página (footer) de la página web de **Akutangulo**, diseñado con una animación SVG para el logotipo y un estilo moderno y minimalista. El footer incluye un logo animado y un texto de copyright dinámico.

### Descripción

El código crea un pie de página centrado con el logotipo de **Akutangulo** en formato SVG, animado con un efecto de trazado (`draw`) y relleno (`fill`). También incluye un texto de copyright con enlaces a la página oficial y un año dinámico actualizado mediante JavaScript. El diseño es limpio, con un fondo oscuro y transiciones suaves para los enlaces.

### Características

- **Animación SVG**: Efectos de trazado (`draw-akutangulo`) y relleno (`fillLogo-akutangulo`) para el logo, además de un brillo dinámico (`glow`).
- **Texto dinámico**: Año de copyright actualizado automáticamente con JavaScript.
- **Responsividad**: Diseño centrado y adaptable a diferentes tamaños de pantalla.
- **Interactividad**: Enlaces con efecto de hover que aumenta el tamaño del texto.
- **Fuentes personalizadas**: Utiliza la fuente `bauhouse_akutangulo` (debe estar definida externamente).
- **Colores personalizables**: Uso de variables CSS como `--color-footer-akutangulo`.

---

📄 Licencia
Este proyecto está bajo la licencia MIT, lo que significa que puedes usarlo libremente en tus proyectos.
