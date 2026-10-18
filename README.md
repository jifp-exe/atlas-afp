# Atlas de carteras de los fondos de pensiones de Chile

Visualizador interactivo de la cartera desagregada de los Fondos de Pensiones A–E
(mayo 2016 en adelante): mapa de la cartera con detalle por instrumento y emisor,
evolución, rentabilidad y riesgo (VaR, CVaR, caída máxima) y derivados (swaps y forwards).

**Ver el sitio:** abra la página de GitHub Pages de este repositorio (Settings → Pages),
o descargue el repositorio y abra `index.html` con doble clic: funciona sin servidor.

## Fuentes
- Superintendencia de Pensiones: cartera desagregada mensual (XML) y valores cuota diarios.
- UF diaria (mindicador.cl) y tasas del Tesoro de EE.UU. (FRED).

La metodología, las correcciones de calidad de datos y el diccionario de códigos están
en la pestaña **Método y diccionario** del visualizador.

## Contenido
- `index.html`: el visualizador (página completa).
- `app.html`: fuente de la página (la arma `pipeline/paso4_html.py` del proyecto).
- `datos/`: datos comprimidos por mes (`mes/AAAA-MM.js`), base, índice y rentabilidad.
- `lib/`: copia local de ECharts para uso sin conexión.

Estos archivos se generan automáticamente; no se editan a mano.
