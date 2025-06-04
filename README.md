
**📁 Bookmark – Gestor de Marcadores**

---

![Hero Illustration](img/illustration-hero.svg)

---

## 🔖 Descripción

**Bookmark** es un gestor de marcadores sencillo, limpio y responsivo que te permite organizar tus sitios web favoritos de forma rápida. Incluye una interfaz atractiva, pestañas de características interactivas y una sección de preguntas frecuentes. Está diseñado con **HTML5**, **SCSS/CSS**, **JavaScript** y **Bootstrap 5**, y cuenta con soporte para compilar estilos desde archivos SCSS.

---

## 🎯 Características principales

- **Interfaz Intuitiva**  
  Diseño minimalista que facilita el acceso a tus marcadores en un solo clic.  
  ![Vista de características](img/illustration-features-tab-1.svg)

- **Pestañas Interactivas de Funcionalidades**  
  - **Simple Bookmarking**: Añade y organiza marcadores arrastrando con soltura.  
  - **Speedy Searching**: Búsqueda ágil de marcadores gracias al filtrado rápido.  
  - **Easy Sharing**: Comparte tus marcadores favoritos con un solo clic.

- **Descarga de Extensiones**  
  Sección para instalar la extensión en los navegadores más populares (Chrome, Firefox y Opera).  
  ![Descarga de extensiones](img/logo-chrome.svg)

- **Preguntas Frecuentes (FAQ)**  
  Acordeón con las dudas más comunes sobre el uso de Bookmark, ampliable a futuras preguntas.

- **Formulario de Suscripción**  
  Mantente al día con las novedades suscribiéndote por correo en el pie de página.

---

## 🖼️ Capturas de Pantalla

<div align="center">
  <img src="img/illustration-hero.svg" alt="Hero Section" width="60%" style="margin-bottom: 1rem;">
  <p>Sección Hero – Información principal y botones de descarga</p>
</div>

<div align="center">
  <img src="img/illustration-features-tab-2.svg" alt="Speedy Searching" width="60%" style="margin-bottom: 1rem;">
  <p>Pestaña “Speedy Searching” – Búsqueda rápida de marcadores</p>
</div>

<div align="center">
  <img src="img/illustration-features-tab-3.svg" alt="Easy Sharing" width="60%" style="margin-bottom: 1rem;">
  <p>Pestaña “Easy Sharing” – Comparte con tus amigos</p>
</div>

<div align="center">
  <img src="img/logo-firefox.svg" alt="Card Firefox" width="100px" style="margin: 0 1rem;">
  <img src="img/logo-chrome.svg" alt="Card Chrome" width="100px" style="margin: 0 1rem;">
  <img src="img/logo-opera.svg" alt="Card Opera" width="100px" style="margin: 0 1rem;">
  <p>Sección de Extensiones – Chrome, Firefox y Opera</p>
</div>

---

## 📂 Estructura del Proyecto

```
bookmark/
├── css/
│   └── main.css
├── img/
│   ├── illustration-hero.svg
│   ├── illustration-features-tab-1.svg
│   ├── illustration-features-tab-2.svg
│   ├── illustration-features-tab-3.svg
│   ├── logo-bookmark.svg
│   ├── logo2-bookmark.svg
│   ├── logo-chrome.svg
│   ├── logo-firefox.svg
│   ├── logo-opera.svg
│   ├── icon-hamburger.svg
│   ├── icon-close.svg
│   ├── bg-dots.svg
│   ├── icon-facebook.svg
│   └── icon-twitter.svg
├── js/
│   └── main.js
├── scss/
│   └── styles.scss
├── css/
│   └── main.css
├── index.html
├── package.json
├── main.css.map
└── README.md
```

- **index.html**: Estructura principal con encabezado, secciones de características, descarga, FAQ y pie de página.
- **scss/styles.scss**: Variables y estilos base organizados en SCSS.
- **css/main.css**: Archivo compilado de estilos, resultado de convertir SCSS a CSS.
- **js/main.js**: Lógica para el menú móvil y cambio de imágenes en las pestañas de características.
- **img/**: Carpetas de ilustraciones, logotipos y recursos gráficos.
- **package.json**: Scripts para compilar SCSS.
- **main.css.map**: Mapa de fuente automática generado durante la compilación de SCSS.

---

## ⚙️ Tecnologías y Dependencias

- **HTML5**  
- **SCSS**  
- **CSS3**  
- **JavaScript (ES6+)**  
- **Bootstrap 5**  
- **Sass (para compilar SCSS)**  

**Dependencias de desarrollo (package.json):**
```json
{
  "scripts": {
    "build-css": "npx sass scss/styles.css css/main.css --no-source-map",
    "watch-css": "sass --watch scss/styles.css css/main.css --no-source-map"
  }
}
```

---

## 🚀 Instalación y Puesta en Marcha

1. **Clonar repositorio**  
   ```bash
   git clone https://github.com/tu-usuario/bookmark.git
   cd bookmark
   ```

2. **Instalar dependencias**  
   No se requieren dependencias adicionales, excepto **Sass** (ya incluido en los scripts). Ejecuta:
   ```bash
   npm install
   ```

3. **Compilar SCSS**  
   - Para compilar una sola vez:
     ```bash
     npm run build-css
     ```
   - Para compilar en modo “watch” (automático):
     ```bash
     npm run watch-css
     ```

   Esto generará/actualizará `css/main.css` según los cambios realizados en `scss/styles.scss`.

4. **Abrir en el navegador**  
   Abre `index.html` en tu navegador preferido (Chrome, Firefox u Opera).  
   ```bash
   open index.html
   ```
   O simplemente haz doble clic sobre el archivo en tu explorador.

---

## 📱 Responsive

Este proyecto está cuidadosamente diseñado para dispositivos móviles y desktops:

- **Menú hamburguesa**: 
  - En pantallas pequeñas (<576px), el menú se expande a pantalla completa con fondo semitransparente y lista vertical de opciones.
  - Elementos responsivos adaptan tamaño de fuentes, espaciados y ocultación de botones no esenciales.

- **Tarjetas de Extensión**:
  - En pantallas grandes (>992px), cada tarjeta (Chrome, Firefox, Opera) tiene un margen escalonado (`.card-step-1`, `.card-step-2`, `.card-step-3`) para crear un efecto visual atractivo.
  - En pantallas pequeñas, las tarjetas ocupan el 100% del ancho y se apilan verticalmente con sombras sutiles.

- **Formulario de Suscripción**:
  - Se centra vertical y horizontalmente; en móviles, ancho del campo de email se ajusta al 60% para mantener estética.

---

## 🔧 Personalización

- **Colores**:  
  Definidos en `:root` y variables SCSS:  
  ```scss
  :root {
    --primary:           #5265E1;
    --secondary:         #FA5959;
    /* ... más variables de color ... */
  }
  ```

- **Tipografía**:  
  Fuente “Inter” desde Google Fonts, importada en `<head>` de `index.html`.

- **Botones**:  
  - `.btn-primary`: Color principal (azul), esquinas redondeadas, transición de hover que invierte colores.  
  - `.btn-secondary`: Color secundario (rojo), hover que invierte colores.  
  - `.btn-grey`: Botones grises con sombra, hover suave.

- **Acordeón (FAQ)**:  
  Basado en el componente de Bootstrap 5.  
  ```html
  <div class="accordion" id="accordionExample">
    <!-- Item 1 -->
    <div class="accordion-item">
      <h2 class="accordion-header" id="headingOne">...
  </div>
  ```

- **JavaScript** (`js/main.js`):
  ```js
  // Cambiar imagen de la pestaña de características
  function changeImages(fileName){
    const img = document.querySelector("#bannerImage");
    img.setAttribute("src", fileName);
  }

  // Menú móvil
  const menu     = document.querySelector('nav ul');
  const openBtn  = document.querySelector('#menu-open');
  const closeBtn = document.querySelector('#menu-close');

  openBtn.addEventListener('click', () => {
    menu.classList.add('open');
  });
  closeBtn.addEventListener('click', () => {
    menu.classList.remove('open');
  });
  ```

---

## 📈 Buenas Prácticas y Salud del Proyecto

- **SCSS Modular**:  
  Aprovecha variables y mixins para mantener consistencia de colores y tipografías.  
- **Mapas de Fuente (source maps)**:  
  El `main.css.map` facilita la depuración en el navegador, relacionando CSS compilado con SCSS original.
- **Bootstrap 5**:  
  - Asegura compatibilidad con múltiples navegadores y diseño responsive sin esfuerzo.  
  - Componentes predefinidos (botones, acordeón, cards) aceleran el desarrollo.

---

## 🛠️ Próximas Mejoras

- **Expansión a más navegadores Chromium**  
  Añadir tabs y tarjetas para Brave, Edge y Vivaldi.
- **Modo Oscuro**  
  Implementar una paleta de colores adaptable y switcher en tiempo real.
- **Login/Logout**  
  Integrar autenticación para que cada usuario tenga su propia colección de marcadores.
- **Funcionalidad de Etiquetas**  
  Permitir clasificar marcadores con etiquetas y buscador avanzado.
- **Estructura de Archivos SCSS**  
  Refactorizar en módulos parciales (`_variables.scss`, `_buttons.scss`, `_layout.scss`, etc.) para mayor escalabilidad.

---

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas!  
1. Haz un _fork_ de este repositorio.  
2. Crea una rama con tu mejora (`git checkout -b feature/nueva-funcionalidad`).  
3. Realiza tus cambios y haz un _commit_ (`git commit -m "Añade nueva función X"`).  
4. Empuja tu rama (`git push origin feature/nueva-funcionalidad`).  
5. Abre un _Pull Request_ detallando las modificaciones.

---

## 📜 Licencia

Este proyecto se distribuye bajo la licencia **MIT**.  
Consulta el archivo `LICENSE` para más detalles.

---

**🌟 Gracias por visitar Bookmark!**

Si tienes preguntas o sugerencias, abre un _issue_ o contáctanos directamente. ¡Esperamos que disfrutes organizando tus marcadores con esta interfaz limpia y eficiente!
