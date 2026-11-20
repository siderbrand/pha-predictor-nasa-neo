# PHA Predictor — Potentially Hazardous Asteroid

Clasificación binaria de asteroides potencialmente peligrosos (PHA) a partir de variables físicas y de aproximación de la NASA.
Proyecto de aula de **Modelos y Simulación de Sistemas II** — Universidad de Antioquia.

**Integrantes:** Eliana Maria Brand Agudelo, Jilberth Ferney Alzate Castaño, Juan Esteban Gil Quintero.

## Contenido

| Archivo | Descripción |
|---|---|
| `informe/informe.tex` | Fuente LaTeX del informe en plantilla IEEE (Entregable II, incluye el Entregable I), con sus figuras en `informe/figuras/`: descripción del problema, estado del arte, metodología, resultados, reducción de dimensión, evaluación final en prueba y conclusiones. |
| `reporte.pdf` | Informe compilado. |
| `entregable1.ipynb` | Secciones I y II del informe (descripción del problema, validación de unidades y estado del arte): reproduce sus cifras, tablas y figuras. |
| `entregable2.ipynb` | Secciones III a VII (metodología, resultados, modelo definido, reducción de dimensión, evaluación final en prueba y conclusiones): reproduce sus cifras, tablas y figuras. El conjunto de prueba solo se usa en la sección 5, con el modelo ya definido. |
| `neo.csv` | Datos: [NASA – Nearest Earth Objects](https://www.kaggle.com/datasets/sameepvani/nasa-nearest-earth-objects) (Kaggle, S. Vani; licencia CC0, dominio público). 90 836 filas, 10 variables. |

Los notebooks no escriben archivos. Ya incluyen sus resultados ejecutados, así que pueden leerse sin volver a correrlos.

## Cómo reproducir

1. Instalar las dependencias:
   ```bash
   pip install numpy pandas scipy scikit-learn matplotlib seaborn umap-learn jupyter
   ```
2. Abrir cada notebook desde la carpeta del repositorio (`neo.csv` debe quedar junto a ellos) y ejecutarlo completo ("Run All"):
   ```bash
   jupyter notebook entregable1.ipynb
   jupyter notebook entregable2.ipynb
   ```
   `entregable1.ipynb` tarda segundos. `entregable2.ipynb` usa todos los núcleos disponibles: con 12 núcleos toma unos 30 minutos y con uno solo varias horas (UMAP no se paraleliza dentro de cada ajuste).
