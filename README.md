# Huellas de fuego, raíces de vida · Tenerife 2027

Web estática promocional para GitHub Pages, adaptable a móvil. Incluye programa de tres días, mapas interactivos Leaflet con los dos GPX aportados y enlaces externos a la ruta de Chanajiga y servicios relacionados.

## Publicar en GitHub Pages

1. Crea un repositorio público en GitHub (por ejemplo `tenerife-2027`).
2. Sube **el contenido de esta carpeta** a la raíz del repositorio, conservando `routes/`.
3. En **Settings → Pages → Build and deployment**, selecciona **Deploy from a branch**, rama `main`, carpeta `/(root)` y guarda.
4. Abre la dirección que GitHub indique, normalmente `https://TU-USUARIO.github.io/tenerife-2027/`.

## Datos del proyecto de clase

- **Tipo de actividad:** proyecto de clase para alumnado del Felo Monzón; **no se comercializa al público**.
- **Precio indicado:** 200 € por persona.
- **Incluye:** billetes de barco de ida y vuelta entre Gran Canaria y Tenerife, coche de alquiler, dos noches en el Hotel Rural Casablanca (Icod el Alto) con media pensión y seguro de viaje.
- **Contacto:** travesia@gmail.com (enlace `mailto:` listo para usar).
- **Almuerzo del tercer día:** visita a Casa Tomás prevista en el programa; no consta expresamente incluido en los 200 €.
- **Fechas:** 27–29 de enero de 2027, conforme al guion oficial del proyecto. Otro archivo muestra por error «27.-29.02.27».
- **Por verificar por la organización:** horarios y reservas de barco, alojamiento, transporte, entradas a Forestal Park, comida en Casa Tomás, permisos, previsión meteorológica, disponibilidad de rutas y seguridad. La web no recibe pagos ni recopila datos de participantes.
- **Imágenes:** recursos visuales CSS originales sin fotografías externas.

## Estructura

- `index.html`: estructura y textos
- `styles.css`: diseño responsive
- `script.js`: pestañas del mapa y botón de contacto
- `routes/*.geojson`: trazas cartográficas generadas desde los GPX originales
- `routes/*.gpx`: descargas originales renombradas

Para probar el mapa localmente, abre una terminal en la carpeta y ejecuta `python -m http.server 8000`; después visita `http://localhost:8000`. Abrir el HTML con doble clic puede impedir que el navegador cargue los GeoJSON.

La cartografía base usa OpenStreetMap y Leaflet mediante internet.


## Corrección de visualización del mapa
Se ha añadido una fuente alternativa de CSS de Leaflet (jsDelivr) y límites de desbordamiento del mapa. Si sigue desajustado, comprueba la conexión a los CDN y recarga con Ctrl+F5.
