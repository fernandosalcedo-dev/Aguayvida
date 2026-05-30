# El Río Habla — Cuenca del Río Indio

Plataforma interactiva de monitoreo de calidad de agua · Autoridad del Canal de Panamá · 2025

## Estructura del proyecto

```
rio-indio-app/
│
├── index.html              ← Landing page: mapa + puntos interactivos
├── rios.html               ← Página de ríos (próxima)
├── metodologia.html        ← Infografía del proceso (próxima)
├── servicios.html          ← Servicios ecosistémicos (próxima)
├── encuesta.html           ← Encuesta comunitaria (próxima)
│
├── assets/
│   └── mapa_cuenca.jpg     ← Mapa oficial de la cuenca (ACP)
│
└── fotos/
    ├── sitios/             ← Fotos de los 17 puntos AS
    │   ├── README.md
    │   ├── AS-1_foto1.jpg  (agregar)
    │   ├── AS-1_foto2.jpg  (agregar)
    │   ├── AS-2_foto1.jpg  (agregar)
    │   └── ...hasta AS-17
    │
    └── rios/               ← Fotos de los 5 ríos
        ├── README.md
        ├── rio_indio_1.jpg     (agregar)
        ├── rio_teria_1.jpg     (agregar)
        ├── rio_uracillo_1.jpg  (agregar)
        ├── rio_la_encantada_1.jpg (agregar)
        └── rio_el_jobo_1.jpg   (agregar)
```

## Cómo agregar fotos

### Fotos de sitios de monitoreo

Nombrar los archivos exactamente así:

```
AS-1_foto1.jpg    ← foto principal del punto de monitoreo
AS-1_foto2.jpg    ← foto del entorno / paisaje
AS-2_foto1.jpg
...
```

La app los carga automáticamente. Si el archivo no existe, muestra un placeholder.

### Fotos de ríos

```
rio_indio_1.jpg
rio_teria_1.jpg
rio_uracillo_1.jpg
rio_la_encantada_1.jpg
rio_el_jobo_1.jpg
```

## Puntos de monitoreo

| ID    | Comunidad             | Tramo | Río              | BMWP | ICA |
|-------|-----------------------|-------|------------------|------|-----|
| AS-1  | Alto de la Mesa       | Alto  | Río Indio        | 165  | 86  |
| AS-2  | Los Chorros           | Alto  | Río Indio        | 161  | 85  |
| AS-3  | Alto del Silencio     | Medio | Río Indio        | 155  | 83  |
| AS-4  | Boca de Uracillo      | Medio | Río Indio        | 150  | 82  |
| AS-5  | El Jobo               | Medio | Río Indio        | 152  | 81  |
| AS-6  | El Cajón              | Bajo  | Río Indio        | 103  | 78  |
| AS-7  | Teriá Nacimiento      | Alto  | Río Teriá        | 165  | 85  |
| AS-8  | Santa Rosa No.1       | Medio | Río Teriá        | 150  | 83  |
| AS-9  | Tres Hermanas         | Medio | Río Teriá        | 150  | 80  |
| AS-10 | Las Canoas            | Medio | Río Uracillo     | 155  | 82  |
| AS-11 | Las Marías            | Medio | Río Uracillo     | 152  | 82  |
| AS-12 | Boca Uracillo         | Medio | Río Uracillo     | 152  | 82  |
| AS-13 | Alcarreto             | Medio | Río La Encantada | 103  | 83  |
| AS-14 | Las Cruces            | Bajo  | Río La Encantada | 98   | 81  |
| AS-15 | La Encantada          | Bajo  | Río La Encantada | 98   | 80  |
| AS-16 | Guayabalito           | Bajo  | Río El Jobo      | 102  | 79  |
| AS-17 | Pablón                | Bajo  | Qda. Pabloncito  | 115  | 81  |

## Fuente de datos

Línea Base Ambiental — Actualización periodo lluvioso 2025  
Elaborado por: URS Holdings / AECOM para la Autoridad del Canal de Panamá  
Campañas: octubre–noviembre 2025  

## Cómo servir localmente

```bash
# Python
python3 -m http.server 8080

# Node
npx serve .
```

Abrir en el navegador: `http://localhost:8080`

> Las fotos no cargan con `file://`. Usar siempre un servidor local o GitHub Pages.

## GitHub Pages

1. Subir todo el contenido a un repositorio GitHub
2. Settings → Pages → Source: `main` / `root`
3. La app queda en `https://usuario.github.io/nombre-repo/`
