# 🚀 Nexus Tech - Blog y Portal de Periodismo Tecnológico

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/es/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/es/docs/Web/CSS)
[![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)](https://git-scm.com/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/)

Bienvenido al repositorio oficial del proyecto **Nexus Tech** (Proyecto Skill HTML & CSS). Este sitio web es una plataforma digital de periodismo tecnológico moderno y minimalista, desarrollada con estándares de accesibilidad, maquetación semántica en HTML5 y un sistema de estilos avanzado en Vanilla CSS3.

A diferencia de la mayoría de portales tecnológicos de tonos oscuros, **Nexus Tech** adopta una **estética Pastel Light Tech**, combinando tonos neutros suaves (`#f8f7f4`, `#ffffff`) con acentos en azul pastel (`#6ea8dc`, `#e8f2fc`), tipografías modernas (*Space Grotesk*, *Poppins*, *Lora*) y micro-animaciones interactivas.

---

## 📌 Tabla de Contenidos

1. [Descripción del Proyecto](#-descripción-del-proyecto)
2. [Estructura del Proyecto y Carpetas](#-estructura-del-proyecto-y-carpetas)
3. [Secciones y Funcionalidades](#-secciones-y-funcionalidades)
4. [Diseño Adaptativo y Responsividad](#-diseño-adaptativo-y-responsividad)
5. [Tecnologías Utilizadas](#-tecnologías-utilizadas)
6. [Flujo de Trabajo y Git](#-flujo-de-trabajo-y-git)
7. [Instrucciones de Ejecución Visual](#-instrucciones-de-ejecución-visual)
8. [Créditos y Licencia](#-créditos-y-licencia)

---

## 📖 Descripción del Proyecto

**Nexus Tech** ha sido diseñado para proporcionar una experiencia de lectura fluida, intuitiva y atractiva en cualquier pantalla. El proyecto incluye 6 vistas principales completamente integradas y navegables entre sí:

* **Inicio (`index.html`)**: Presentación del portal, banner hero con llamada a la acción y tarjetas de noticias con desplegables interactivos de contenido.
* **Categorías (`pages/categorias.html`)**: Catálogo estructurado de 15 artículos en cuadrícula con panel lateral fijo (sticky) de filtros por tema/fecha y simulación de paginación.
* **Reseñas (`pages/resenas.html`)**: Análisis a fondo de gadgets con calificaciones en estrellas, tabla comparativa técnica de productos y sección de comentarios de la comunidad.
* **Comunidad (`pages/comunidad.html`)**: Tarjetas con contadores de usuarios, foro de discusión maquetado, sidebar de tendencias y preguntas frecuentes (FAQ) en formato acordeón.
* **Eventos (`pages/eventos.html`)**: Calendario interactivo visual de lanzamientos/conferencias y lista de eventos mundiales destacados con enlaces oficiales reales.
* **Contacto (`pages/contacto.html`)**: Formulario con validaciones visuales CSS, tarjetas con información detallada, mapa estático de ubicación y botones de redes sociales con efectos 3D.

---

## 📁 Estructura del Proyecto y Carpetas

El proyecto cuenta con una arquitectura de archivos modular y organizada siguiendo la metodología BEM y separando las hojas de estilo por componente/sección:

```text
Proyecto_Skill_HTML_CSS_NexusTech/
├── assets/
│   └── img/                         # Imágenes optimizadas del sitio (.webp, .jpg, .png)
│       ├── Banner-img.png
│       ├── agentes-autonomos.jpg
│       ├── audifonos.jpg
│       ├── baterias.webp
│       ├── ciberseguridad.webp
│       ├── expo.webp
│       ├── gpt5.webp
│       ├── maps.png
│       ├── notebook.webp
│       ├── pulse.jpg
│       ├── smartwatch.webp
│       └── ...
├── css/                             # Hojas de estilo modulares
│   ├── main.css                     # Variables CSS globales, colores pastel, tipografía y CSS Reset
│   ├── style.css                    # Encabezado sticky, menú hamburguesa responsivo, banner y footer global
│   ├── categorias.css               # Estilos del sidebar sticky, grid de artículos y paginación
│   ├── resenas.css                  # Estilos de tarjetas de reseñas, tabla comparativa y formulario/comentarios
│   ├── comunidad.css                # Estilos del foro, tabla de temas, estadísticas y FAQ acordeón
│   ├── eventos.css                  # Estilos del calendario visual y tarjetas de eventos destacados
│   └── contacto.css                 # Estilos del formulario de contacto y tarjetas de redes sociales animadas
├── pages/                           # Vistas secundarias del portal
│   ├── categorias.html              # Página de categorías y filtros
│   ├── resenas.html                 # Página de reseñas y comparativas
│   ├── comunidad.html                # Página de foro y comunidad
│   ├── eventos.html                 # Página de agenda y calendario
│   └── contacto.html                # Página de contacto y ubicación
├── index.html                       # Página de inicio principal
└── README.md                        # Documentación principal del proyecto
```

---

## 🛠️ Secciones y Funcionalidades

### 1. Página de Inicio (`index.html`)
* **Header & Navbar Sticky**: Encabezado superior persistente con efecto de desfoque de vidrio (*glassmorphism*), logotipo con acento pastel y menú de navegación.
* **Menú Hamburguesa Responsivo (CSS-Only)**: Sistema dinámico mediante `<input type="checkbox">` que convierte las 3 barras en una **'X'** y despliega un menú flotante en dispositivos móviles (`< 768px`).
* **Banner Hero**: Presentación de las tendencias 2026 con insignias, título llamativo, descripción y botones CTA hacia noticias y categorías. Acompañado de la tarjeta de la historia destacada con imagen de portada.
* **Tarjetas Expandibles Interactivas**: Tarjetas de artículos con desplegables `<details>` y `<summary>` que muestran resúmenes extendidos y puntos clave mediante una animación fluida (`expandFadeIn`), sin redirigir al usuario fuera de la vista principal.
* **Footer Global**: Pie de página de 4 columnas con información institucional, navegación rápida, enlaces a categorías, datos de contacto y redes sociales animadas.

### 2. Página de Categorías (`pages/categorias.html`)
* **Sidebar de Filtros Sticky**: Panel fijo a la izquierda (`position: sticky`) con filtros visuales por temas (*IA, Gadgets, Ciberseguridad, Desarrollo, Tendencias*) y antigüedad (*7 días, 30 días, Más antiguos*).
* **Cuadrícula de 15 Artículos**: Organizada en 3 columnas flexibles (escritorio), 2 (tablets) y 1 (móviles) utilizando **CSS Grid**, sin estrellas ni puntuaciones para mantener la diferencia conceptual con las reseñas.
* **Paginación Simulada**: Control visual al final de la página con botones "Anterior", "Siguiente" y números de página con efectos hover en azul pastel.

### 3. Página de Reseñas (`pages/resenas.html`)
* **Tarjetas de Análisis**: Presentación de productos tecnológicos (*NovaBook Air 14, Pulse X Pro, AuraSound Elite, Chrono Watch 3*) con calificación en estrellas (`★`), score numérico e imagen.
* **Tabla Comparativa Técnica**: Matriz responsiva (`<table class="table-container__products">`) con especificaciones clave, estimación de precios y puntuación general, con resaltado de filas mediante `:hover`.
* **Comentarios y Opiniones**: Formulario lateral para ingresar valoraciones y lista de comentarios recientes de la comunidad.

### 4. Página de Comunidad (`pages/comunidad.html`)
* **Contadores de Usuarios**: 4 tarjetas de estadísticas con métricas de la comunidad (*+45K Miembros, 120K Debates, etc.*).
* **Foro de Discusión**: Tabla maquetada de temas con íconos de colores pastel por categoría, autores, respuestas, vistas y fecha de última actividad.
* **Acordeón FAQ**: Preguntas frecuentes construidas con `<details class="faq-item">` y rotación animada de ícono `+` a `×`.

### 5. Página de Eventos (`pages/eventos.html`)
* **Calendario de Eventos**: Rejilla mensual de días con etiquetas clasificadoras según el tipo de evento (*Conferencia, Lanzamiento, Meetup*).
* **Eventos Destacados**: Tarjetas con información oficial de convenciones reales (*CES Las Vegas 2027, MWC Barcelona 2027, Apple WWDC 2026, Google I/O 2026*) con enlaces directos a sus portales oficiales (`target="_blank"`).

### 6. Página de Contacto (`pages/contacto.html`)
* **Formulario con Validaciones Visuales**: Campos obligatorios con pseudo-clases CSS (`:required`, `:focus`, `:valid`) para indicar estado mediante bordes y sombras pastel.
* **Redes Sociales Animadas**: Botones con colores institucionales (*Twitter/X, LinkedIn, GitHub, YouTube, Instagram*) que reaccionan al cursor con rotación de íconos, elevación 3D e iluminación brillante.
* **Mapa de Ubicación**: Tarjeta contenedora con la imagen estática de la sede en Bucaramanga, Colombia.

---

## 📱 Diseño Adaptativo y Responsividad

El sitio web fue construido bajo los principios de diseño responsivo adaptativo, garantizando la correcta visualización en diversas resoluciones de pantalla:

| Dispositivo | Ancho de Pantalla | Comportamiento del Layout |
| :--- | :--- | :--- |
| **Escritorio Grande** | `> 1024px` | Grids de 3 o 4 columnas, sidebars fijos en pantalla y barra de navegación extendida. |
| **Tablets** | `768px - 1024px` | Grids adaptados a 2 columnas, sidebars apilados verticalmente y layout compacto. |
| **Smartphones / Móviles** | `< 768px` | Grids de 1 columna (100% ancho), menú hamburguesa desplegable y padding ajustado a `92vw`. |

---

## 💻 Tecnologías Utilizadas

* **HTML5**: Maquetación semántica (`<header>`, `<nav>`, `<main>`, `<article>`, `<aside>`, `<section>`, `<footer>`, `<details>`, `<summary>`).
* **CSS3 (Vanilla)**:
  * **Variables CSS Globales (`:root`)**: Control unificado de paleta de colores pastel, sombras, tipografía y radios de borde.
  * **Layout Moderno**: Combinación de **CSS Grid** (`grid-template-columns`, `gap`) y **Flexbox**.
  * **Animaciones Keyframes & Transiciones**: Efectos suaves al pasar el mouse (`transform: translateY()`, `scale()`, `rotate()`).
  * **Media Queries**: Ajustes finos de Breakpoints para móviles (`768px`, `640px`, `1024px`).
* **Git & GitHub**: Control de versiones estructurado mediante ramas (*feature branches*) y mensajes según **Conventional Commits**.

---

## 🔀 Flujo de Trabajo y Git

El desarrollo del proyecto siguió una estrategia de ramificación basada en funcionalidades (`feature branches`) antes de consolidar el código final en la rama principal de desarrollo (`develop`):

* `feature/pagina-inicio`: Maquetación, banner hero, tarjetas expandibles y footer.
* `feature/pagina-categorias`: Sidebar de filtros, grid de 15 productos y paginación.
* `feature/pagina-reseñas`: Tarjetas de reseñas con score, tabla comparativa y comentarios.
* `feature/pagina-comunidad`: Métricas de usuario, tabla de foro y FAQ interactivo.
* `feature/pagina-eventos`: Calendario visual de eventos y tarjetas de eventos globales.
* `feature/pagina-contacto`: Formulario con validaciones, tarjetas de información y redes sociales animadas.

> **Nota:** Todos los commits emplean el estándar de **Conventional Commits** (ejemplo: `:lipstick:feat(pagina-inicio): navbar responsiva con menu hamburguesa interactivo para moviles`).

---

## ⚡ Instrucciones de Ejecución Visual

Para visualizar y probar el proyecto localmente en tu equipo:

1. **Clonar el Repositorio**:
   ```bash
   git clone https://github.com/JulianValenciaRv0/Proyecto_Skill_HTML_CSS_NexusTech.git
   ```

2. **Acceder al Directorio**:
   ```bash
   cd Proyecto_Skill_HTML_CSS_NexusTech
   ```

3. **Abrir en el Navegador**:
   * Simplemente haz doble clic sobre el archivo `index.html` para abrirlo en cualquier navegador web moderno (Google Chrome, Mozilla Firefox, Microsoft Edge, Safari).
   * O si usas **VS Code**, instala la extensión **Live Server**, haz clic derecho sobre `index.html` y selecciona **"Open with Live Server"**.

---

## 👤 Autor

* **Julián Valencia** - *Desarrollo HTML5 & CSS3* - [GitHub Repository](https://github.com/JulianValenciaRv0/Proyecto_Skill_HTML_CSS_NexusTech)

---
*© 2026 Nexus Tech. Proyecto desarrollado para la certificación Skill HTML/CSS.*
