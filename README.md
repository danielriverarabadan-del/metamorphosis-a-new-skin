# METAMORPHOSIS — A NEW SKIN

Sitio estático responsive, sin tienda ni dependencias de ejecución. Incluye las fotografías, el video de renders y los cuatro pasaportes digitales entregados.

## Abrir el sitio desde este paquete

Descomprime el ZIP completo y abre `index.html` con Chrome, Edge o Firefox. Conserva la carpeta `assets` junto al archivo HTML para que carguen las fotos, el video y los PDF. Con conexión a internet también se carga la tipografía Manrope/DM Mono usada en el diseño.

## Reemplazar los recursos

- **Fotografías:** las imágenes recibidas ya están en `assets/images/` y conectadas en `index.html`. `fig-01-general-1.jpg` corresponde a `GENERAL - 1`; las cuatro piezas usan `cornu-collection.jpg`, `elytra-collection.png`, `tarsus-collection.jpg` y `metamer-collection.jpg` (la imagen original venía nombrada “ÉLITRA”). Todas las demás imágenes quedaron en la galería como `sesion-*`. Para reemplazar una, conserva el nombre de archivo y sobrescríbela.
- **Video:** el video recibido ya está en `assets/video/renders.mp4` y conectado al reproductor con controles. Para reemplazarlo, conserva ese nombre y sustituye el archivo. Para agregar un póster, añade `poster="assets/images/poster.jpg"` al elemento `<video>` de `index.html`.
- **Pasaportes:** los cuatro PDF recibidos ya están dentro de `assets/passports/` como `cornu.pdf`, `elytra.pdf`, `tarsus.pdf` y `metamer.pdf`. Los enlaces abren cada PDF en una pestaña nueva; desde el visor del navegador se puede descargar.

Mantén las rutas relativas para que funcione tanto localmente como en hosting estático. Puedes cambiar textos y títulos directamente en `index.html`; colores, tipografía y espaciado están en `styles.css`.

## Probar en local

Abre una terminal en esta carpeta y ejecuta `py -m http.server 8000` (o `python -m http.server 8000`). Visita `http://localhost:8000`. Detén el servidor con Ctrl+C. También puedes abrir `index.html` directamente, aunque el servidor local reproduce mejor el comportamiento de publicación.

## Publicar gratis

**GitHub Pages** ofrece alojamiento gratuito para este sitio estático: crea un repositorio público en GitHub, sube el contenido de esta carpeta y, en el repositorio, abre **Settings → Pages**. En “Build and deployment” elige **Deploy from a branch**, selecciona `main` y la carpeta `/ (root)`, y guarda. GitHub mostrará el enlace público del sitio al terminar el despliegue. Usa la URL que aparece en esa pantalla para compartirla. Si ya tienes GitHub, no se requiere comprar dominio ni agregar servicios.
