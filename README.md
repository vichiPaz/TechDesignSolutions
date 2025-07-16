# TechDesign Solutions - Desarrollo de Interfaz de Usuario Web

Este proyecto se enfoca en el desarrollo de una interfaz de usuario web modular, escalable y responsiva para TechDesign Solutions, una plataforma de comercio electrónico. El objetivo es mejorar la experiencia del usuario y aumentar las tasas de conversión mediante la implementación de prácticas modernas de desarrollo front-end.

## Tecnologías Utilizadas

- **HTML5**
- **CSS3** (con preprocesador SASS)
- **JavaScript**
- **Bootstrap 4**
- **Metodología BEM (Bloque Elemento Modificador)** para la estructuración de CSS

## Funcionalidades Implementadas

Basado en los requisitos del proyecto, se han implementado las siguientes características y metodologías clave:

### Metodología BEM

- El código CSS está estructurado siguiendo la metodología BEM para componentes claros, modulares y reutilizables.
- Los nombres de las clases se adhieren a las convenciones BEM (Bloque\_\_Elemento--Modificador).
- Se evita el uso de selectores excesivamente anidados y selectores de etiquetas directos para mantener la especificidad y la reutilización.
- Se aplican convenciones de nomenclatura consistentes en todo el proyecto.

### Preprocesadores CSS (SASS)

- SASS se utiliza como preprocesador CSS para mejorar la mantenibilidad y organización.
- Los estilos se dividen en archivos parciales (`.scss`) para una mejor modularidad (ej., `abstracts`, `components`, `pages`).
- Se utilizan variables extensivamente para definir colores, fuentes y otros valores reutilizables.
- Se implementan mixins para evitar la repetición en los estilos.

### Modelo de Caja

- Todos los elementos siguen correctamente el modelo de caja.
- Se utiliza `box-sizing: border-box;` para facilitar el cálculo de dimensiones.
- Uso eficiente de `padding` y `margin` para un espaciado adecuado entre elementos.

### Integración de Bootstrap 4

- Se utiliza el sistema de cuadrícula de Bootstrap 4 para estructuras de layout responsivas.
- Se integran componentes de Bootstrap como botones, formularios y tarjetas.
- La personalización de los estilos de Bootstrap se logra mediante variables SASS cuando es necesario.

## Estructura del Proyecto

```
TechDesignSolutions/
├───dist/                 # Archivos CSS compilados
│   └───styles.css
├───public/               # Activos estáticos (JS, imágenes) - Los archivos HTML fueron movidos a la raíz
│   ├───assets/
│   │   └───img/
│   │       └───wave.jpg
│   └───js/
│       ├───bootstrap.bundle.min.js
│       ├───bootstrap.min.js
│       └───script.js
├───src/
│   └───scss/             # Archivos fuente SASS
│       ├───main.scss
│       ├───abstracts/
│       │   ├───_mixins.scss
│       │   └───_variables.scss
│       ├───components/
│       │   ├───_button.scss
│       │   ├───_card.scss
│       │   ├───_footer.scss
│       │   └───_nav.scss
│       └───pages/
│           ├───_contact.scss
│           └───_home.scss
├───contact.html          # Página de contacto (movida desde public/)
├───index.html            # Punto de entrada principal (movido desde public/)
├───package.json          # Dependencias y scripts del proyecto
├───package-lock.json
└───README.md             # Documentación del proyecto
```

## Instalación y Configuración

Para configurar el proyecto localmente, siga estos pasos:

1.  **Clonar el repositorio:**

    ```bash
    git clone https://github.com/vichiPaz/TechDesignSolutions.git
    cd TechDesignSolutions
    ```

2.  **Instalar dependencias:**

    ```bash
    npm install
    ```

3.  **Compilar SASS:**
    Para compilar los archivos SASS y observar los cambios, ejecute:
    ```bash
    npm run sass
    ```
    Este comando compilará `src/scss/main.scss` en `dist/styles.css` y recompilará automáticamente los cambios.

## Uso

Abra `index.html` en su navegador web para ver el proyecto. La página `contact.html` también está disponible.

## Despliegue

Este proyecto está diseñado para ser fácilmente desplegable en servicios de alojamiento de sitios estáticos como GitHub Pages, Netlify o Vercel. Los archivos `index.html` y `contact.html` se encuentran en el directorio raíz para una configuración de despliegue sencilla.

## Desarrollado por

Valentina Troncoso Molina

vtroncosomolina@gmail.com
