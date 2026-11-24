# KevinTV Player — LG QA Demo

Lista M3U de prueba para certificación LG webOS. **No contiene suscripciones IPTV ni contenido comercial**.

## URL M3U para el portal
https://raw.githubusercontent.com/kevintv-player/kevintv-demo/main/demo_lg.m3u

## Grupos provisionales
- 01 TV Demo: 2 entradas
- 02 Peliculas Demo: 2 entradas
- 03 Series Demo: 2 entradas

**Todas las entradas utilizan temporalmente la misma fuente:** Big Buck Bunny (c) 2008 Blender Foundation — [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/). Fuente: https://peach.blender.org/ . Se debe conservar la atribución en usos posteriores.

> Importante: en KevinTV C3g, los grupos M3U se presentan como categorías de TV en vivo. No equivalen a categorías VOD de películas ni a temporadas de series.

Para sustituir el video, cambiar solo la URL inmediatamente posterior a la línea `#EXTINF` correspondiente, manteniendo intacta la estructura.

Los links tienen que apuntar a un recurso MP4/HLS directo reproducible en webOS: un enlace para compartir de Drive o una página de Vimeo no suele ser suficiente.

No se ha comprobado aún la reproducción ni el acceso CORS al archivo MP4 en un televisor LG. Probar antes de remitir esta fuente a LG QA.
