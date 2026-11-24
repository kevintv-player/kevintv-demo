# KevinTV Player — LG QA Demo

Lista M3U pública de prueba para LG webOS. URL para el portal:

https://raw.githubusercontent.com/kevintv-player/kevintv-demo/main/demo_lg.m3u

## Estado de la prueba (24 noviembre 2026)

- 2 entradas TV, 2 Películas y 2 episodios Serie, con sintaxis M3U extendida clásica `#EXTINF`, `tvg-id`, `tvg-name`, `tvg-logo`, `group-title`.
- 5 entradas apuntan al MP4 `flower.mp4` de MDN (CC0), que el usuario verificó reproduciendo en KevinTV C3h.
- La película 01 apunta a `https://media.w3.org/2010/05/sintel/trailer.mp4`, una nueva fuente candidata MP4 que **falta probar en webOS**.
- Se retiraron por ahora los enlaces a Google Cloud Storage que el usuario reportó como no reproducibles.
- La película 01 utiliza nombre correcto «Sintel - Tráiler de prueba» y no lleva la portada anterior de Big Buck Bunny para evitar atribución visual equivocada.
- Los demás títulos e imágenes son marcadores de demostración; no representan videos diferentes.

## Próximos pasos
Sincronizar la misma lista en el emulador. Probar la película 01 (W3C) y una entrada Demo 02 (MDN). Si W3C no reproduce, cambiar solo su URL por el enlace MDN comprobado, sin modificar la aplicación.

Esta lista es para pruebas técnicas; no es una biblioteca de certificación final. La compatibilidad de URLs depende de la respuesta del host, codificación y condiciones de reproducción en LG webOS.

Referencia licencia Blender Sintel: https://studio.blender.org/films/sintel/
MDN: https://interactive-examples.mdn.mozilla.net/media/cc0-videos/flower.mp4
