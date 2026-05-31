# 🌲 Markup Converter — ArcGIS Field Maps
 
**Convierte archivos `.markup` de ArcGIS Field Maps a KML y GeoJSON directamente en el navegador.**
 
---
 
## El origen de esta herramienta
 
Todo empezó con una petición real de un técnico de campo de mi empresa.
 
ArcGIS Field Maps permite crear **marcas personales**: dibujos de áreas, líneas y puntos en el mapa, con distintos colores, completamente privados. Son anotaciones personales que solo ve el propio usuario y que no están alojadas como capas en ArcGIS Online, sino vinculadas al dispositivo y al perfil local de la app.
 
El problema: **si cambias de dispositivo o se reinicia el perfil de Field Maps, las pierdes**. Y su formato `.markup` es propietario de Esri — no lo lee ninguna otra aplicación directamente.
 
La petición fue concreta:
- Poder **exportarlas** para no perderlas
- Convertirlas a **KML** para abrirlas en Google Earth
- Poder **compartirlas con otros compañeros** o usarlas en aplicaciones distintas cuando están en campo
---
 
## La solución
 
Una pequeña app web que resuelve exactamente eso: subes el `.markup`, eliges el formato y descargas el archivo convertido. Sin instalaciones, sin servidores, sin cuentas.
 
### Por qué una web app y no otra cosa
 
- Las empresas suelen tener **filtros de seguridad estrictos** que bloquean enlaces o aplicaciones desconocidas
- Los técnicos de campo trabajan a menudo **sin cobertura de red**
- No todo el mundo tiene Python o herramientas GIS en su equipo
La versión publicada aquí es **100% offline una vez cargada**: todo el procesamiento ocurre en el navegador del usuario, ningún dato sale del dispositivo.
 
---
 
## Qué hace
 
- 📂 Carga archivos `.markup` exportados desde ArcGIS Field Maps
- 🔄 Reproyecta automáticamente de Web Mercator (EPSG:3857) a WGS84
- 🌍 Exporta a **KML** (Google Earth, ArcGIS, etc.)
- 🗺️ Exporta a **GeoJSON** (QGIS, visores web, etc.)
- ✅ Compatible con polígonos, líneas y puntos
- 📱 Funciona en móvil, tablet y escritorio
---
 
## Cómo usarla
 
👉 [**cmlg96.github.io/markup-converter**](https://cmlg96.github.io/markup-converter)
 
1. Exporta tu markup desde Field Maps (compartir → guardar archivo)
2. Abre la web y arrastra el archivo `.markup`
3. Elige KML, GeoJSON o ambos
4. Descarga y usa donde necesites
---
 
## Reflexión final
 
Lo que me parece más valioso de este proceso no es la herramienta en sí, sino lo que la originó: **la curiosidad de querer resolver el problema real de alguien**.
 
Quienes trabajamos con GIS tenemos la responsabilidad — y la oportunidad — de tender puentes entre las herramientas y las personas que las usan en campo. Herramientas como la IA nos permiten hacerlo más rápido y mejor, siempre que sepamos hacer las preguntas correctas y pensar en quién va a usar lo que construimos.
 
---

 

