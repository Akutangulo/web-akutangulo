# Página web de Akutangulo.com
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

## Footer Akutangulo 
Footer de Akutangulo.com para mostrar en las webs

---

📄 Licencia
Este proyecto está bajo la licencia MIT, lo que significa que puedes usarlo libremente en tus proyectos.
