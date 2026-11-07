# MINERVA Launcher · PWA

Prototipo web instalable en Android desde el navegador, sin APK.

## Publicar en GitHub Pages

1. Crea un repositorio en GitHub (por ejemplo `minerva-launcher`).
2. Sube **todo el contenido** de esta carpeta a la raíz del repositorio:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - carpeta `icons/`
3. En GitHub abre **Settings → Pages**.
4. En **Build and deployment**, selecciona `Deploy from a branch`.
5. Selecciona la rama `main` y la carpeta `/ (root)`, y guarda.
6. Espera a que GitHub Pages publique la web. La URL tendrá normalmente esta forma:
   `https://TU-USUARIO.github.io/minerva-launcher/`

## Instalar en Android

1. Abre la URL publicada con Chrome en Android.
2. Espera a que cargue una vez con conexión.
3. Abre el menú de Chrome (⋮).
4. Pulsa **Instalar aplicación** o **Añadir a pantalla de inicio** (el texto depende de la versión de Chrome).
5. MINERVA aparecerá como acceso independiente, sin barra del navegador.

## Qué incluye

- `index.html`: interfaz del prototipo.
- `manifest.json`: identidad y configuración de instalación PWA.
- `sw.js`: service worker y caché básica para abrir la interfaz sin conexión tras la primera carga.
- `icons/`: iconos de la aplicación.

## Límites de esta versión

- No es un APK ni una aplicación Android nativa.
- El modo offline conserva la interfaz; no incorpora todavía catálogos, servicios multimedia ni controles reales.
- Las preferencias de visibilidad se guardan en el almacenamiento local del navegador/dispositivo.
- El service worker requiere HTTPS; GitHub Pages lo proporciona automáticamente.
- Para actualizar la caché tras cambiar archivos, incrementa `minerva-shell-v1` en `sw.js` (por ejemplo, `v2`).

## Privacidad

Esta versión no incorpora analítica, telemetría, cuentas ni conexiones externas. La caché y las preferencias permanecen en el dispositivo.
