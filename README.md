# Proyecto-Final-Carcelero

Proyecto completo para el Proyecto Final de CoderHouse - Desarrollo Web.

## Nombre del Proyecto

**Musa Store** - Tienda de ropa básica

## Cómo ejecutarlo

1. Clona o descarga este repositorio en tu computadora.
2. Abre el archivo `index.html` en tu navegador web preferido.
3. O bien, puedes usar un servidor local:
   - Si tienes Python instalado: `python -m http.server 8000`
   - Si tienes Node.js instalado: `npx http-server`
   - Luego accede a `http://localhost:8000` en tu navegador

## Compilar SCSS a CSS

Este proyecto utiliza SASS/SCSS como preprocesador de CSS. Para compilar los archivos SCSS:

### Opción 1: Usando npm (recomendado)

1. Instala las dependencias:
```bash
npm install
```

2. Compila el SCSS (incluye source maps para debugging):
```bash
npm run sass
```

3. Para compilar en modo watch (recompila automáticamente al guardar cambios):
```bash
npm run sass:watch
```

4. Para compilar en modo comprimido (producción):
```bash
npm run sass:compressed
```

**Nota:** Todos los scripts generan source maps (`.map`) que permiten debuggear el código SCSS original desde las herramientas de desarrollo del navegador.

### Opción 2: Usando sass directamente

Si tienes sass instalado globalmente:

```bash
sass scss/main.scss css/styles.css
```

Para modo watch:
```bash
sass --watch scss/main.scss css/styles.css
```

## Cómo subirlo a GitHub

1. Crea un nuevo repositorio en GitHub con el nombre `PreEntrega2_Carcelero`.
2. Abre una terminal en la carpeta del proyecto.
3. Ejecuta los siguientes comandos:

```bash
git init
git add .
git commit -m "Initial commit - PreEntrega 2"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/PreEntrega2_Carcelero.git
git push -u origin main
```

**Nota:** Reemplaza `TU_USUARIO` con tu nombre de usuario de GitHub.

## Cómo activar GitHub Pages

1. Ve a tu repositorio en GitHub.
2. Haz clic en **Settings** (Configuración).
3. En el menú lateral, selecciona **Pages** (Páginas).
4. En **Source** (Origen), selecciona la rama `main` y la carpeta `/root`.
5. Haz clic en **Save** (Guardar).
6. Espera unos minutos y tu sitio estará disponible en:
   `https://facucarcelero.github.io/PreEntrega2-Carcelero/`

## Estructura del Proyecto

```
PreEntrega3_Carcelero/
├─ index.html              # Página principal
├─ pages/
│  ├─ about.html           # Página sobre nosotros
│  ├─ catalogo.html        # Catálogo de productos
│  ├─ contacto.html        # Formulario de contacto
│  ├─ galeria.html         # Galería de imágenes
│  └─ servicios.html       # Lista de servicios
├─ css/
│  ├─ styles.css           # Estilos compilados (generado desde SCSS)
│  └─ styles.css.map       # Source map para debugging (generado desde SCSS)
├─ scss/                   # Archivos fuente SCSS
│  ├─ abstracts/          # Variables, mixins, functions
│  │  ├─ _variables.scss
│  │  ├─ _mixins.scss
│  │  └─ _functions.scss
│  ├─ base/               # Reset, tipografía
│  │  ├─ _reset.scss
│  │  └─ _typography.scss
│  ├─ components/         # Componentes reutilizables
│  │  ├─ _buttons.scss
│  │  ├─ _cards.scss
│  │  ├─ _navbar.scss
│  │  ├─ _badges.scss
│  │  ├─ _alerts.scss
│  │  ├─ _breadcrumb.scss
│  │  └─ _pagination.scss
│  ├─ layout/             # Layout principal
│  │  ├─ _header.scss
│  │  ├─ _footer.scss
│  │  ├─ _grid.scss
│  │  └─ _main.scss
│  ├─ pages/              # Estilos específicos por página
│  │  ├─ _index.scss
│  │  ├─ _catalogo.scss
│  │  └─ _about.scss
│  ├─ themes/             # Temas
│  │  └─ _theme.scss
│  ├─ vendors/            # Overrides de librerías
│  │  └─ _bootstrap-overrides.scss
│  └─ main.scss           # Archivo principal que importa todo
├─ assets/
│  └─ img/                 # Imágenes del proyecto
├─ wireframes/
│  └─ PreEntrega2+Carcelero-wireframes.pdf
├─ package.json           # Configuración npm y scripts
├─ README.md               # Este archivo
└─ .gitignore             # Archivos ignorados por Git
```

## Tecnologías Utilizadas

- HTML5
- CSS3 / SCSS (SASS Preprocessor)
- Bootstrap 5 (CDN)
- Git y GitHub
- Node.js / npm (para compilar SCSS)

## Características

- ✅ Diseño responsive (mobile, tablet, desktop)
- ✅ Navegación unificada en todas las páginas
- ✅ Uso de etiquetas semánticas HTML5
- ✅ Bootstrap 5 para componentes y grid
- ✅ SCSS/SASS con arquitectura 7-1 pattern
- ✅ Variables, mixins, @extend y operadores SASS
- ✅ Transiciones, transformaciones y animaciones avanzadas
- ✅ CSS Grid real (no solo Bootstrap)
- ✅ Formulario de contacto funcional (HTML)
- ✅ Galería de imágenes con grid Bootstrap
- ✅ Catálogo de productos con cards
- ✅ Media queries con unidades relativas
- ✅ Source maps para debugging SCSS
- ✅ Optimización para producción

## Características SCSS Implementadas

### Arquitectura 7-1 Pattern
- **Abstracts**: Variables, mixins y funciones reutilizables
- **Base**: Reset y tipografía base
- **Components**: Componentes modulares (botones, cards, navbar, etc.)
- **Layout**: Estructura principal (header, footer, grid, main)
- **Pages**: Estilos específicos por página
- **Themes**: Configuración de temas
- **Vendors**: Overrides de librerías externas (Bootstrap)

### Funcionalidades SASS
- ✅ **Variables**: Colores, espaciados, breakpoints, transiciones
- ✅ **Mixins**: Responsive, transiciones, animaciones, hover effects
- ✅ **@extend**: Reutilización de estilos base
- ✅ **Operadores**: Cálculos matemáticos, loops con @each y @for
- ✅ **Nesting**: Estructura anidada clara y organizada
- ✅ **Funciones**: Cálculos y transformaciones de valores

### Animaciones y Efectos
- Fade in / Slide up en elementos
- Hover effects con transformaciones
- Animaciones pulse para badges y botones
- Transiciones suaves en todos los componentes
- Delay escalonado para cards y grid items

## Optimización y Mejores Prácticas

### Source Maps
El proyecto incluye source maps (`.css.map`) que permiten:
- Debuggear el código SCSS original desde las DevTools del navegador
- Ver exactamente qué archivo SCSS generó cada regla CSS
- Facilitar el desarrollo y mantenimiento del código

Los source maps se generan automáticamente al compilar con los scripts de npm.

### Optimización de Imágenes
Para mejorar el rendimiento del sitio, se recomienda:
- Comprimir imágenes antes de subirlas (herramientas: TinyPNG, ImageOptim, Squoosh)
- Usar formatos modernos como WebP cuando sea posible
- Ajustar el tamaño de las imágenes al tamaño de visualización necesario
- Considerar usar `loading="lazy"` en imágenes que no están en el viewport inicial

### Testing Cross-Browser
El proyecto ha sido probado y funciona correctamente en:
- Chrome/Edge (últimas versiones)
- Firefox (últimas versiones)
- Safari (últimas versiones)
- Navegadores móviles (iOS Safari, Chrome Mobile)

**Herramientas recomendadas para testing:**
- BrowserStack
- CrossBrowserTesting
- DevTools de navegadores (modo responsive)

### GitHub Pages
Para verificar que GitHub Pages está activado:
1. Ve a Settings → Pages en tu repositorio
2. Verifica que la fuente esté configurada (rama `main`, carpeta `/root`)
3. El sitio debería estar disponible en: `https://TU_USUARIO.github.io/PreEntrega2-Carcelero/`
4. Puedes verificar el estado en la pestaña "Actions" si está habilitado

## Autor

Desarrollado para la Pre-Entrega 3 de CoderHouse - Desarrollo Web.

---

**Nota:** Este proyecto utiliza Bootstrap 5 a través de CDN, por lo que requiere conexión a internet para cargar los estilos y scripts de Bootstrap. Los archivos SCSS deben compilarse a CSS antes de usar el proyecto.
