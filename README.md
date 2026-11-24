# KevinTV Player — LG QA Demo

Lista M3U de prueba para LG webOS, sin contenido comercial.

**URL de lista (para portal KevinTV):** https://raw.githubusercontent.com/kevintv-player/kevintv-demo/main/demo_lg.m3u

## Estructura (seis entradas)
- TV Demo: 2 entradas, `tvg-type="live"`
- VOD | Peliculas: 2 entradas, `tvg-type="movie"`
- VOD | Series: 2 entradas, `tvg-type="series"`

Cada entrada tiene `tvg-id`, `tvg-name`, `tvg-type`, `tvg-logo`, `group-title` y una URL MP4.

**Fuentes provisionales para aislar errores de reproduccion: Big Buck Bunny (c) 2008 Blender Foundation, licencia CC BY 3.0, alojado en el bucket de pruebas GTV de Google; y el clip CC0 `flower.mp4` de MDN. Los seis elementos alternan estas dos fuentes para contrastar resultados. Las etiquetas de catalogo son provisionales.

**Limitación confirmada de KevinTV C3g:** El parser M3U actual interpreta todas las entradas como live TV e ignora `tvg-type`; devuelve listas vacías para `get_vod_categories`, `get_vod_streams`, `get_series_categories` y `get_series`. Añadir atributos a esta lista NO habilita las pestañas Películas/Series de esa versión. Se requiere soporte adicional en el reproductor o una fuente Xtream real para habilitarlas.

Para cambiar contenidos, sustituir la URL situada inmediatamente después del `#EXTINF` correspondiente. Verificar que los enlaces sean directos y reproducibles por webOS; un enlace compartido de Drive puede no serlo.

## Prueba de reproduccion (noviembre 2026)
La lista alterna tres URLs `https://storage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4` y tres URLs `https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4`. No se ha probado aun en el emulador/televisor LG. Esta mezcla es temporal, no material final de certificacion. Si falla solo una fuente, revisar el servidor o la compatibilidad de ese MP4; si fallan ambas, revisar el reproductor y el codigo de error concreto.
