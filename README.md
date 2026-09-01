# Convergencia en el modelo de Solow

Página web interactiva de una sola vista con tres simuladores para clase:

1. **Trayectoria temporal** — cómo converge `k(t)` al estado estacionario.
2. **Diagrama clásico** — función de producción, curva de ahorro `s·f(k)` y recta de depreciación `(δ+n)k`.
3. **β-convergencia y σ-convergencia** — 12 economías simuladas con distinto capital inicial, mostrando la relación entre crecimiento e ingreso inicial, y la dispersión entre economías en el tiempo.

No tiene dependencias de build: es un único archivo `index.html` que carga Chart.js desde un CDN. Se puede abrir localmente haciendo doble clic, o publicarlo en internet gratis con GitHub Pages.

## Subir el proyecto a GitHub

Necesitás tener [Git](https://git-scm.com/downloads) instalado y una cuenta de GitHub.

1. Creá un repositorio nuevo en GitHub (por ejemplo `solow-convergencia`), **sin** inicializarlo con README (para no pisar el que ya tenés acá).
2. En tu computadora, dentro de esta carpeta, corré:

```bash
git init
git add .
git commit -m "Simuladores de convergencia del modelo de Solow"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/solow-convergencia.git
git push -u origin main
```

Reemplazá `TU-USUARIO` por tu nombre de usuario de GitHub.

## Publicarlo con GitHub Pages (para que tu amigo solo abra un link)

1. En GitHub, andá al repositorio → **Settings** → **Pages**.
2. En "Build and deployment" → "Source", elegí **Deploy from a branch**.
3. En "Branch", elegí **main** y la carpeta **/ (root)**. Guardá.
4. Esperá uno o dos minutos. GitHub va a mostrar la URL pública, con esta forma:

```
https://TU-USUARIO.github.io/solow-convergencia/
```

Ese link funciona en cualquier proyector o computadora con internet — ideal para mostrarlo en clase. Si tu amigo va a hacer cambios (por ejemplo, ajustar rangos de los sliders o los colores), puede editar directamente `index.html`; cualquier `git push` a `main` actualiza la página publicada en un par de minutos.

## Uso sin internet / sin GitHub

Si preferís no depender de conexión durante la clase, alcanza con abrir `index.html` en el navegador. Lo único que requiere internet es la carga de Chart.js y las tipografías desde el CDN — si vas a usarlo sin conexión, conviene abrirlo una vez con internet antes para que el navegador cachee esos recursos, o descargar Chart.js localmente y ajustar el `<script src="...">` en `index.html`.
