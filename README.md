# Grafo de colaboración de Margot Robbie

Parte individual del proyecto final de Análisis y Ciencia de Datos, Universidad del Istmo.
Sofía Isabela Sandoval Vásquez.

Con datos de The Movie Database (TMDB) se arma el grafo de colaboración de Margot Robbie
(películas de 1975 a 2025 en las que el actor sale con `order < 5`) y se estudia con el
espectro de su Laplaciano normalizado: componentes, brecha espectral, clustering espectral,
vector de Fiedler y centralidad.

## Archivos

```
grafo_margot_robbie.ipynb   notebook con todo (clases Graph y TMDBAPIUtils, grafo y espectro)
cache/                      respuestas del API en JSON
figs/grafo.png              figura del grafo
figs/grafo_comunidades.png  grafo coloreado por comunidad espectral
figs/espectro.png           primeros 15 valores propios de Lsym
```

## Cómo correrlo

    pip install -r requirements.txt
    jupyter nbconvert --to notebook --execute --inplace grafo_margot_robbie.ipynb

Corre sin API key, sólo con `cache/`. Para descargar de nuevo, se guarda el key en
`tmdb_key.txt` (está en `.gitignore`).

## Uso de IA

Me apoyé en IA (Claude) para armar la estructura de las clases `Graph` y `TMDBAPIUtils`
y del cache, para el código del espectro y para dar formato a las figuras. Las respuestas
del notebook las analicé yo y la IA sólo ayudó con la redacción.
