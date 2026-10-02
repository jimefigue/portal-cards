# Web Estática con Cards - GitHub Pages

Sitio web estático multinivel diseñado con tarjetas interactivas de tamaño uniforme y navegación fluida.

## 🚀 Estructura de Navegación

1. **Home (`index.html`)**:
   - 6 tarjetas temáticas (MARCAS, Estabilidad, Bocetos, Médica, Bioequivalencia, EVPT MAPT).
   - Al hacer click en cada una, redirige a su página correspondiente (`pages/page-X/index.html`).

2. **Páginas de Sección (`pages/page-X/index.html`)**:
   - Cada una contiene 2 tarjetas (1, 2) con el **mismo tamaño exacto** que las de la Home.
   - Breadcrumbs y botón para regresar a Inicio.
   - Al hacer click en cada tarjeta, redirige a su página de detalle (`card-1.html` o `card-2.html`).

3. **Páginas de Detalle (`pages/page-X/card-Y.html`)**:
   - Muestra el contenido con texto **Lorem Ipsum** estructurado y estilizado.
   - Navegación rápida para volver a la sección o al inicio.

---

## 🌐 Publicación en GitHub Pages

Este proyecto ya cuenta con el archivo de configuración `.nojekyll` y el flujo automatizado `.github/workflows/deploy.yml`.

### Pasos para publicar:

1. **Crear o conectar tu repositorio en GitHub:**
   ```bash
   git remote add origin https://github.com/<tu-usuario>/<tu-repositorio>.git
   ```

2. **Confirmar los cambios y subir al repositorio:**
   ```bash
   git add .
   git commit -m "feat: sitio web estático multinivel con cards y deploy a gh-pages"
   git branch -M main
   git push -u origin main
   ```

3. **Activar GitHub Pages en el repositorio:**
   - Ve a tu repositorio en GitHub: **Settings** > **Pages**.
   - En **Build and deployment** > **Source**, selecciona:
     - **GitHub Actions** (se desplegará automáticamente con el workflow incluido).
     - *O alternativamente:* **Deploy from a branch**, seleccionando la rama `main` y la carpeta `/ (root)`.
   - En unos segundos tu sitio estará disponible en:
     `https://<tu-usuario>.github.io/<tu-repositorio>/`
