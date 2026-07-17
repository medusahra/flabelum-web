# Flabelum — sitio web

Sitio estático (HTML/CSS/JS, sin frameworks) listo para publicar en GitHub Pages.

## Estructura
```
index.html          → todo el sitio (una sola página con secciones ancladas)
images/              → ilustraciones placeholder (reemplazar por tus fotos)
```

## Cómo subirlo a tu GitHub (paso a paso)

### 1. Crear el repositorio
1. Andá a https://github.com/new
2. Nombre del repositorio: **`flabelum`** (o el que prefieras — si querés que quede en `tunombre.github.io/flabelum`, cualquier nombre sirve; si querés que sea la raíz de un dominio tipo `flabelum.github.io`, el repo se debe llamar exactamente `flabelum.github.io` — pero eso solo funciona si tu usuario de GitHub se llama `flabelum`, así que lo más simple es un nombre normal como `flabelum-web`).
3. Público, sin licencia ni README (ya tenés uno).
4. Click en **Create repository**.

### 2. Subir los archivos
Opción fácil (sin terminal):
1. En la página del repo recién creado, click en **"uploading an existing file"**.
2. Arrastrá `index.html` y la carpeta `images/` completa.
3. Commit directo a `main`.

Opción con terminal, desde la carpeta del proyecto:
```bash
git init
git add .
git commit -m "Sitio Flabelum"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/flabelum-web.git
git push -u origin main
```

### 3. Activar GitHub Pages
1. En el repo, andá a **Settings → Pages**.
2. En "Build and deployment" → **Source**, elegí **Deploy from a branch**.
3. **Branch**: `main`, carpeta `/ (root)`. Guardar.
4. Esperá 1–2 minutos. Tu sitio queda en:
   `https://TU-USUARIO.github.io/flabelum-web/`

### 4. Reemplazar las fotos
Cuando me pases tus fotos, las voy a preparar en el mismo formato (cuadradas, fondo neutro)
y reemplazamos `images/piece-1.svg` … `piece-4.svg` y `images/about-me.svg` por tus
`.jpg`/`.webp` reales — solo hay que cambiar el `src` en `index.html` (una línea por pieza)
y volver a subir el archivo al repo.

### 5. Dominio propio (opcional)
Si más adelante querés `flabelum.com` en vez de la URL de github.io, en
**Settings → Pages → Custom domain** se agrega el dominio y se configuran los DNS
del proveedor donde lo compres. Avisame cuando llegue ese momento y te guío.
