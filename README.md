# Visor de Wikimapia por comuna — O'Higgins

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![OpenStreetMap](https://img.shields.io/badge/OpenStreetMap-7EBC6F?style=flat-square&logo=openstreetmap&logoColor=white)

Herramienta web **autocontenida** que consulta la **API de Wikimapia** y muestra
los objetos (lugares) registrados por cada una de las 33 comunas de la Región de
O'Higgins, sobre un mapa. Los límites comunales se obtienen al vuelo desde
**OpenStreetMap / Nominatim**, sin necesidad de cargar archivos.

## ¿Qué hace?

- Consulta Wikimapia comuna por comuna y filtra los lugares contra el polígono
  comunal real.
- Resuelve el transporte de la API antigua con **descubrimiento automático de
  JSONP** (prueba variantes de callback hasta encontrar la que funciona) y
  soporte opcional de proxy para publicación en HTTPS.
- Permite "contar las 33" comunas para obtener solo los totales, con control de
  ritmo entre consultas.

## Stack

- HTML / CSS / JavaScript (sin build, funciona vía `file://`)
- [MapLibre GL JS](https://maplibre.org/)
- API de Wikimapia · OpenStreetMap (Nominatim/Overpass)

## Uso

1. Abre `VIZ_WIKIMAPIA_OHIGGINS_SELECTOR.html` en el navegador.
2. Ingresa tu clave de Wikimapia (gratis en
   [wikimapia.org/api](https://wikimapia.org/api/?action=my_keys)) o usa la clave
   de demo `example`.
3. Elige una comuna y consulta.

## Créditos de datos

Lugares: colaboradores de Wikimapia (CC BY-SA). Límites comunales: OpenStreetMap
vía Nominatim (ODbL).

## Nota

Desarrollado con asistencia de IA.
