## 1.Definición

Un **generador de sitios estáticos** (SSG, del inglés *Static Site Generator*) es una herramienta que crea una página web completa en HTML, CSS y JavaScript a partir de archivos más sencillos, como textos y plantillas. El resultado es un sitio formado por archivos ya construidos, sin base de datos ni código que ejecutar en el servidor.

## 1.1. Para qué sirve

Sirve para crear webs de forma más cómoda y organizada, sin escribir todo el HTML a mano. Se utiliza sobre todo en proyectos cuyo contenido no cambia constantemente:

- Blogs y webs personales.
- Documentación técnica y manuales.
- Portfolios y páginas de presentación.
- Webs informativas o institucionales de contenido estable.

## 1.2. Archivos que utiliza como punto de partida

- **Contenido:** archivos de texto en Markdown (.md), donde se escribe cada página o entrada.
- **Plantillas:** archivos que definen el diseño común del sitio (cabecera, menú, pie de página) y dónde se insertará el contenido.
- **Configuración:** archivos en YAML, JSON o TOML con los datos generales del sitio (título, idioma, menús, rutas).
- **Recursos estáticos:** imágenes, hojas de estilo CSS y archivos JavaScript.

## 1.3. Cómo transforma esos archivos en una página web

El generador lee el contenido escrito en Markdown, lo convierte a HTML y lo inserta dentro de las plantillas. De este modo, todas las páginas comparten el mismo diseño pero mantienen su contenido propio. El resultado final es una carpeta con los archivos HTML, CSS, JavaScript e imágenes listos para subir a un servidor.

## 1.4. En qué momento se genera el HTML

El HTML se genera **antes de publicar la web**, durante el proceso llamado *build* (compilación). No se crea cuando el usuario visita la página: ya está hecho de antemano, por lo que el servidor únicamente tiene que entregar los archivos tal y como están.

## 1.5. Comparación de generadores: Jekyll, Hugo y Astro

| Aspecto | Jekyll | Hugo | Astro |
| ------- | ------ | ---- | ----- |
| **Tecnología principal** | Ruby | Go | JavaScript / TypeScript (Node.js) |
| **Formato del contenido** | Markdown + plantillas Liquid | Markdown + plantillas de Go | Markdown, MDX y componentes .astro |
| **Instalación** | Ruby y la gema Jekyll | Un único ejecutable | Node.js y npm |
| **Funcionamiento básico** | Convierte Markdown en HTML aplicando plantillas | Igual que Jekyll, pero compila mucho más rápido | Genera HTML y solo añade JavaScript donde hace falta |
| **Usos habituales** | Blogs y webs personales | Documentación y sitios con muchas páginas | Blogs, portfolios y webs modernas |
| **Ventajas** | Sencillo e integrado de forma nativa en GitHub Pages | Muy rápido y fácil de instalar | Flexible; permite componentes de React, Vue u otros |
| **Inconvenientes** | Lento cuando el sitio tiene muchas páginas | Sistema de plantillas algo difícil al principio | Requiere conocimientos de JavaScript |
| **Publicación en GitHub Pages** | Sí, de forma nativa | Sí, mediante GitHub Actions | Sí, mediante GitHub Actions |

[Guía de Markdown en vídeo](https://www.youtube.com/watch?v=osWfEtbP_sk)