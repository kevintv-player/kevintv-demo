# KevinTV Player — Biblioteca QA para LG webOS

**URL M3U (se mantiene estable):**

https://raw.githubusercontent.com/kevintv-player/kevintv-demo/main/demo_lg.m3u

## Inventario actual (24 noviembre 2026)

| Sección | Nombre | Fuente | Validación |
|---|---|---|---|
| TV | KevinTV Nature — Flores | MDN flower.mp4 | La fuente MDN se reprodujo en C3h |
| TV | KevinTV Cinema — Animación (Prueba) | Test Videos BBB H.264 720p 10s | **Pendiente de probar en LG** |
| Películas | Big Buck Bunny — Clip 10s (Prueba) | Test Videos BBB H.264 720p 10s | **Pendiente de probar en LG** |
| Películas | Flores — Cortometraje Demo | MDN flower.mp4 | La fuente MDN se reprodujo en C3h |
| Series | Flora Demo S01 E01 | MDN flower.mp4 | La fuente MDN se reprodujo en C3h |
| Series | Flora Demo S01 E02 | MDN flower.mp4 | La fuente MDN se reprodujo en C3h |

### Archivos gráficos
- `assets/logos/kevintv-nature.svg`
- `assets/logos/kevintv-cinema.svg`
- `assets/posters/flores.svg`
- `assets/posters/animacion.svg`
- `assets/posters/serie-flora.svg`

Los gráficos son **ilustraciones vectoriales originales y genéricas de demostración**, no fotogramas oficiales de las películas. Los nombres señalan cuando un contenido es provisional o está pendiente de verificación. Las tarjetas de la serie reutilizan el clip de flores como episodios ficticios de prueba. No se ofrece este material como una obra completa.

### Procedencia y permisos
- **Flower**: ejemplo CC0 de Mozilla Developer Network, `https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4`.
- **Big Buck Bunny**: (c) copyright 2008, Blender Foundation / www.bigbuckbunny.org — CC BY 3.0. En esta demo se prueba un recorte de 10 segundos alojado por `test-videos.co.uk`. Conservar atribución de Blender.

El clip nuevo requiere prueba real en el emulador / TV antes de aprobar la biblioteca LG. El host de terceros no está bajo nuestro control. No usar el clip como material final si falla o si sus condiciones de redistribución no son adecuadas.

### Mantenimiento

Para reemplazar un video, editar únicamente la línea URL posterior a su `#EXTINF` manteniendo `tvg-id`, `tvg-name`, `tvg-logo` y `group-title`. Si cambia la obra, actualizar también nombre, categoría, imagen y créditos. No se modificó la app, el portal, Render ni Supabase.
