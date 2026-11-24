# KevinTV Player — LG QA Demo

Lista M3U de prueba para LG webOS, sin contenido comercial.

**URL de lista (para portal KevinTV):** https://raw.githubusercontent.com/kevintv-player/kevintv-demo/main/demo_lg.m3u

## Estructura (seis entradas)
- TV Demo: 2 entradas, `tvg-type="live"`
- VOD | Peliculas: 2 entradas, `tvg-type="movie"`
- VOD | Series: 2 entradas, `tvg-type="series"`

Cada entrada tiene `tvg-id`, `tvg-name`, `tvg-type`, `tvg-logo`, `group-title` y una URL MP4.

**Origen de prueba:** Big Buck Bunny, (c) 2008 Blender Foundation, licencia [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/). Portada: [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Big_buck_bunny_poster_big.jpg). Conservar atribución. Todas las entradas usan temporalmente el mismo video, solo para probar organización.

**Limitación confirmada de KevinTV C3g:** El parser M3U actual interpreta todas las entradas como live TV e ignora `tvg-type`; devuelve listas vacías para `get_vod_categories`, `get_vod_streams`, `get_series_categories` y `get_series`. Añadir atributos a esta lista NO habilita las pestañas Películas/Series de esa versión. Se requiere soporte adicional en el reproductor o una fuente Xtream real para habilitarlas.

Para cambiar contenidos, sustituir la URL situada inmediatamente después del `#EXTINF` correspondiente. Verificar que los enlaces sean directos y reproducibles por webOS; un enlace compartido de Drive puede no serlo.
